- It is meant to work with Mellow Fly Super8 board with TMC5160 HV on XY and TMC2209 on E and Z

# Note for Super 8 Pro with STM32h723 Chip:
## If you are having random MCU disconnection/shutdown, please switch to software SPI, by commenting out the "spi_bus: spi1a" line on each 5160s section and uncomment those 3 lines:


- spi_software_mosi_pin: PB5 
- spi_software_miso_pin: PB4 
- spi_software_sclk_pin: PB3 

# Useful links:
- Super8 and Super8 Pro Documation: https://teamgloomy.github.io/fly_super8_general.html
- Super8 Std Klipper info: https://mellow.klipper.cn/#/board/fly_super8/
- Super8 Pro Klipper info: https://mellow.klipper.cn/#/board/fly_super8_pro/

# DISCLAIMER
- The macro files are REQUIRED for our printer.cfg to work with klipper.
- Its also REQUIRED to add a "Linux Process" to klipper, See the "Install the rc script" and "Building the micro-controller code" section [https://www.klipper3d.org/RPi_microcontroller.html]

# Macros information: DO NOT USE THE SPEED MACROS WITHOUT READING THIS.
## Speed Macros Explanation
Explanation: 
- 1st line: Steps << number of times it will do the stop and go, 100 times in the below case>>
- 2nd line: Velocity/Speed << The speed/velocity at which you want to test. 1000mms here>>
- 3rd line: safety distance << the safety distance in mm that the print head will not go from X max and Y max defined on your printer config>>	
- 4th line: Starting Accel << the starting acceleration value for the test. 10K here>>	

### Credits to DoubleT on Discord for his help on these macros

 [gcode_macro ACCELL_TEST_X]
 
gcode:

    {% set steps = params.STEPS|default(100)|int %}
    {% set speed = params.VELOCITY|default(1000)|float * 60 %}
    
    {% set inset = 10.0|float %} 
    {% set accel = 10000|int %} 
    {% set maxX = printer.configfile.settings.stepper_x.position_max|float - inset %}
    {% set maxY = printer.configfile.settings.stepper_y.position_max|float - inset %}
    {% set minX = printer.configfile.settings.stepper_x.position_min|float + inset %}
    {% set minY = printer.configfile.settings.stepper_y.position_min|float + inset %}

    SAVE_GCODE_STATE NAME=accelltest_state

    SET_VELOCITY_LIMIT ACCEL={accel} 
    SET_VELOCITY_LIMIT ACCEL_TO_DECEL={accel}
    G28
	G1 Z5
    G1 X{minX} Y{minY} F{speed} 

    {% for INTERVAL in range(steps) %}
        {% set eff = accel + (INTERVAL * 1000) %} 
        SET_VELOCITY_LIMIT ACCEL={eff} 
        SET_VELOCITY_LIMIT ACCEL_TO_DECEL={eff}
        G1 X{minX} Y{minY} F{speed}  
        G1 X{maxX} Y{maxY} F{speed}  

    {% endfor %}    

    RESTORE_GCODE_STATE NAME=accelltest_state 
	
	
	
[gcode_macro ACCELL_TEST_Y]

gcode:

    {% set steps = params.STEPS|default(100)|int %}
    {% set speed = params.VELOCITY|default(1000)|float * 60 %}

    {% set inset = 10.0|float %}
    {% set accel = 10000|int %}
    {% set maxX = printer.configfile.settings.stepper_x.position_max|float - inset %}
    {% set maxY = printer.configfile.settings.stepper_y.position_max|float - inset %}
    {% set minX = printer.configfile.settings.stepper_x.position_min|float + inset %}
    {% set minY = printer.configfile.settings.stepper_y.position_min|float + inset %}

    SAVE_GCODE_STATE NAME=accelltest_state

    SET_VELOCITY_LIMIT ACCEL={accel} 
    SET_VELOCITY_LIMIT ACCEL_TO_DECEL={accel}
    G28
	G1 Z5
    G1 X{minX} Y{minY} F{speed} 

    {% for INTERVAL in range(steps) %}
        {% set eff = accel + (INTERVAL * 1000) %} 
        SET_VELOCITY_LIMIT ACCEL={eff} 
        SET_VELOCITY_LIMIT ACCEL_TO_DECEL={eff}
        G1 X{maxX} Y{minY} F{speed}  
        G1 X{minX} Y{maxY} F{speed}  

    {% endfor %}    

    RESTORE_GCODE_STATE NAME=accelltest_state 
