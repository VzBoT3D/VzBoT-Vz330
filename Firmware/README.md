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
