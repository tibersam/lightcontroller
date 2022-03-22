# Lightcontroller

This is a project to build a controller for SK2812 LEDs.
The microcontroller receives commands from the Kodi Plugin over an RS485 UART, processes the command and calculates the LEDs values, and then sends the LEDs values over an SPI-to-SK2812 interface to the LEDs.
The Microcontroller also recieves commands over an RS232 UART from a Button box to allow control of the LEDs without Kodi.

* In **schematic** you find the shield i designed for the project.
* In **firmware** you find the firmware of the microcontroller.
* In **kodi-plugin** you find the python plugin for kodi
* In **button-box** you find the firmware of the microcontroller in the button box.

It uses the 24 Pin header of a standard ATX power supply as Power source.
The LEDs are split into 3 power sections. One is directly powered by the 5V of the power supply.
The other 2 are powered by two step down converters from 12V to 5V, which i bought online.
In Total i have 432 LEDS which are used for an indirect lighting of the room.
