# RadioHead
RadioHead Packet Radio library for embedded microprocessors from http://www.airspayce.com/mikem/arduino/RadioHead/

**Chnages from aprendiendoarduino**
- This is a github repository for the RadioHead Packet Radio library with a simple modification to use with LoRa modules RFM95.
- Just modified setFrequency(868.0); from setFrequency(434.0); in RH_RF95.cpp file to ease the use with LoRa modules RFM95.
- Also maintain a git version control for the RadioHead Packet Radio library for embedded microprocessors

This is the RadioHead Packet Radio library for embedded microprocessors.
It provides a complete object-oriented library for sending and receiving packetized messages
via a variety of common data radios and other transports on a range of embedded microprocessors.

The version of the package that this documentation refers to can be downloaded 
from http://www.airspayce.com/mikem/arduino/RadioHead/RadioHead-1.83.zip
You can find the latest version of the documentation at http://www.airspayce.com/mikem/arduino/RadioHead

You can also find online help and discussion at 
http://groups.google.com/group/radiohead-arduino

## Overview

RadioHead consists of 2 main sets of classes: Drivers and Managers.

- Drivers provide low level access to a range of different packet radios and other packetized message transports.
- Managers provide high level message sending and receiving facilities for a range of different requirements.

Every RadioHead program will have an instance of a Driver to
provide access to the data radio or transport, and usually a
Manager that uses that driver to send and receive messages for the
application. The programmer is required to instantiate a Driver
and a Manager, and to initialise the Manager. Thereafter the
facilities of the Manager can be used to send and receive
messages.

It is also possible to use a Driver on its own, without a Manager, although this only allows unaddressed, 
unreliable transport via the Driver's facilities.

In some specialised use cases, it is possible to instantiate more than one Driver and more than one Manager.

A range of different common embedded microprocessor platforms are supported, allowing your project to run
on your choice of processor.

Example programs are included to show the main modes of use.

**More information read RadioHead.h file**