# calypso-usb-addon
USB add-on for the Calypso board

# Description
Based on the inexpensive HS8836A USB 2.0 hub, this add-on provides 4 extra USB ports to connect peripherals to the Calypso board. This could come handy to connect USB keyboards and mice or any other device supported by the Calypso firmware.

The board exposes a micro USB connector to connect to the RP2040 with an additional cable (male USB-C to male Micro-USB). 

Be careful to choose a cable with a thin and short connector on the micro-usb side, because the PS/2 connector blocks don't leave much vertical room to accommodate the cable connector.

The board provides power to the USB peripherals coming directly from the Calypso Mini USB port. Take that into account when choosing the power supply for the Calypso board since it must provide enough power for the USB hub and the devices you might connect. 


