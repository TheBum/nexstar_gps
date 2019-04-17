# SkySync GPS clone
 
A project to build an open source Celestron SkySync GPS compatible unit. This variant includes a 128x32 pixel SSD1306 OLED display for showing position, time, and satellite information.
 
Forked from ForestTree's fork of the fantastic project by bebrown (https://github.com/bebrown/nexstar_gps).
 
## Goals
 
Construct a SkySync-compatible unit for attaching a GPS to Celestron mounts that don't already have a GPS, such as the CGEM or AVX.
 
## Parts
 
To build this, you will need:
 
* A GPS module, such as the uBlox NEO-6M. Commonly used by hoobyists for their quadcopters.
  Available for about $16.
 
* A small Arduino, such as the Pro Mini (5V version). Clones available for about $3.
 
* A TTL serial-to-USB adapter for programming the Arduino (if it does not have an on-board
  USB port already). Available for about $3.
 
* A 128x32 pixel (or larger) SSD1306 I2C OLED display.
 
## Construction
 
See [schematics diagram](eagle-Nano/Nano-schematic.png).
 
## Libraries
 
You will need to install the following libraries:
 
* TinyGPS++, available from http://arduiniana.org/libraries/tinygpsplus/.
 
* SSD1306Ascii, available through the Arduino Library Manager.
 
Also needed are the following libraries built in to the Arduino IDE:
 
* SoftwareSerial
 
* Wire
 
## Additional info
 
See this links for more info about Celestron mounts, AUX port, wiring and communication protocol:
 
https://www.nexstarsite.com/download/manuals/NexStarCommunicationProtocolV1.2.zip
https://sites.google.com/site/wayneholder/nexstar-direct-telescope-mount-control
https://www.nexstarsite.com/download/CelestronAS_PCinterface.pdf
http://www.paquettefamily.ca/nexstar/NexStar_AUX_Commands_10.pdf

The eagle-Nano folder contains the EAGLE design files for the schematic and board, as well as a zip archive ready for upload to a PCB service (e.g. https://jlcpcb.com).
 
## Attention
 
Be attentive during construction and testing your device!!! You can easy destroy the motherboard in your astro mount.
