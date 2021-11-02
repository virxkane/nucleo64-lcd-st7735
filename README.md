# nucleo64-lcd-st7735
LCD shield for STM32 Nucleo-64 boards.

This shield is designed for connecting to STM32 Nucleo-64 boards via Arduino<sup>TM</sup> Uno V3.

**WARNING:** Although this shield can be connected to the Arduino<sup>TM</sup> UNO, it is incompatible in logic levels, so it is strictly forbidden to connect this way, otherwise this display will fail!

### Hardware
* The GMT177-01 module is used as a display and is compatible in size and pins. The display controller used is **ST7735**. The display data bus is connected to the hardware SPI. PWM can be used  to control the brightness of the screen backlight.
* Joystick K1-1504SA-03 and one button KLS7-TS6601 can be used for control. Both are connected to 3 General Purpose I / O ports via diodes.
* EEPROM memory M24C08 can be used to store user data. This IC is connected to the I2C hardware bus.
* Two LEDs are connected to ports A0 (PA0) and A1 (PA1).
* A separate button IT-1187-160GM-G is provided to reset the controller.

### Demo firmware
Two versions of the demo firmware have been written to work on the NUCLEO-F446RE and this shield, one using CMSIS, the other using HAL. Both are under BSD-3-Clause License.
* Using CMSIS: [nucleo-f446re-st7735spi-shield](https://github.com/virxkane/nucleo-f446re-st7735spi-shield)
* USING HAL: [nucleo-f446re-st7735spi-shield-hal](https://github.com/virxkane/nucleo-f446re-st7735spi-shield-hal)

