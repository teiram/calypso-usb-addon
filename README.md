# calypso-powerpack-addon (was calypso-usb-addon)
Add-on for the calypso board featuring USB 2.0 hub with 4 ports and 8MB PSRAM

![Preview](https://github.com/teiram/calypso-powerpack-addon/blob/master/calypso-powerpack-addon-preview.png?raw=true)

# Description
Based on the inexpensive HS8836A USB 2.0 hub, this add-on provides 4 extra USB ports to connect peripherals to the Calypso board. This could come handy to connect USB keyboards and mice or any other device supported by the Calypso firmware.

It also provides a footprint to install 8MB of extra PSRAM. The PSRAM is addressed using QSPI and was tested to run properly at 108Mhz clock, what would allow to simulate a 8 bit SRAM at around 148 ns access time. Please take into account that version 0.1 has an error in the silk text and iBOM: The PSRAM to use is a ESP32-PSRAM64H.

The board exposes a micro USB connector to connect to the RP2040 with an additional cable (male USB-C to male Micro-USB). But it would be more practical to solder a cable directly to the provided D+/D- pads on the board. You only need two wires for D+/D- since ground is common and the board powers the USB peripherals.

![With direct cable](https://github.com/teiram/calypso-powerpack-addon/blob/master/calypso-powerpack-addon-installed.jpg?raw=true)


In case you go for the micro-usb connector, try to choose a cable with a thin and short connector on the micro-usb side, because the PS/2 connector blocks don't leave much vertical room to accommodate the cable connector.

For the USB-C side, I recommend to use a connector with presoldered miniboard exposing D+/D-, like the one in the picture.

![With direct cable](https://github.com/teiram/calypso-powerpack-addon/blob/master/usb-c-connector.jpg?raw=true)


The board provides power to the USB peripherals coming directly from the Calypso Mini USB port. Take that into account when choosing the power supply for the Calypso board since it must provide enough power for the USB hub and the devices you might connect. 

# Changelog
- 0.1. Initial version
- 0.2. Fix ibom and silk for PSRAM (ESP-PSRAM64H)

