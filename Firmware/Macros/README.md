# Please use with EXTREME care and keep your finger ready on the Emergency stop or power switch. Print WILL fail and you need to stop it when it fails.

Explanation: 
- 1st line: Steps << number of times it will do the stop and go, 100 times in the below case>>
- 2nd line: Velocity/Speed << The speed/velocity at which you want to test. 1000mms here>>
- 3rd line: safety distance << the safety distance in mm that the print head will not go from X max and Y max defined on your printer config>>	
- 4th line: Starting Accel << the starting acceleration value for the test. 10K here>>	

## Credits to DoubleT on Discord for his help on these macros

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
