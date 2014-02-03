---
title: Communication Information
layout: default
---

# Communication between, from, and how long
<hr>
<br>

## Communication types

+ RS232
+ RS422
+ RS485
+ CAN BUS
+ MOD Bus ( Serial Communication Protocol ).

<br>
<hr>
## Intro

  This page tells you available types of communication protocol, which takes place between microcontrollers or say between a master and slaves.

<hr>

### RS232

<hr>

### RS422


<hr>

### RS485

ANSI TIA EIA - 485 is a standard defining the electrical characteristics of drivers and receivers for use in balanced digital multipoint systems. RS means "Recommended Standard".

Components required - 
+ Max 485 E 
+ [Datasheet here](http://datasheets.maxim-ic.com/en/ds/MAX1487E-MAX491E.pdf)
+ [Available , from element 14](http://in.element14.com/jsp/search/browse.jsp;jsessionid=DDVDTFPQQG0UUCWNBBSRFYY?N=0&Ntk=gensearch&Ntt=MAX485E&Ntx=mode+matchallpartial&exposeLevel2Refinement=true&suggestions=false&ref=globalsearch&_requestid=10151)
+ DIP 8 package - 316 / pcs
+ SOIC 8 package- 250 / pcs
+ The same also availabel in mouser and digikey by part number - MAX 485E.
+ For detailed study and comparisions, [please take a look here](http://www.lammertbies.nl/comm/info/RS-485.html)
+ Its schematics are provided in the datasheet itself.
+ With arduino, wire connection are show below.
<br>
![Alt text](http://dereenigne.org/wp-content/uploads/modbus-417x600.png)
+ Arduino serial [example goes here](http://arduino-info.wikispaces.com/SoftwareSerialRS485Example)
+ Another library with [arduino with max485](https://github.com/Protoneer/RS485-Arduino-Library)
+ About cables, this part is coming soon.

<br>
<hr>
<br>


<hr>

### CAN Bus

+ Controller Area Network (CAN)
+ Originally developed by Robert Bosh.
+ Multi drop, multi master serial bus provides communication between controllers, sensors and actuators.
+ Multi drop, .i.e is, many device on a BUS.
+ CAN 2.0 A is Standard format.
+ CAN 2.0 B is extended format.
+ InternationalStandard ISO 11898
	+ ISO 11898 2 High Speed applications up to 1Mbps.
	+ ISO 11898 3 Low Speed applications up to 125 Kbps
+ CAN broadcast the messages, any node is allowed to broadcast a message.
+ Each message contains an ID that identifies the source, or the contentof a message.
+ Receiver will decide to process or ignore the message, each message.
+ [Check this CAN BUS introduction video.](http://www.youtube.com/watch?v=fTWp6bFIt0s)
+ [CAN Cable characteristics, BUS length 50Kbits per sec for within 1000m range, Screened twisted-pair cables (2x2) with a characteristic impedance of between 108 and 132 Ohm is recommended for the CAN wiring.](http://infosys.beckhoff.com/english.php?content=../content/1033/bx5200/html/co_inswirbus.htm&id=)
+ Available CAN Bus in India
	+ [Protocentral](http://www.protocentral.com/arduino-shields/337-can-bus-shield.html) , for 1,799 INR.
	+ [Sumeet e shop](http://shop.sumeetinstruments.com/index.php?route=product/product&path=69_71&product_id=436), for 3,650 INR.
	+ [entesla](http://entesla.com/mcp2515-SPI-CAN?filter_name=CAN), for 1,100 INR.
+ [Tested with arduino, and interfacing](http://www.seeedstudio.com/wiki/CAN-BUS_Shield)
+ But the above code library is according to the shield.

### A DIY of CAN as a customised board

####Components required
+ MCP2515 CAN Bus controller with SPI interface.
	+ [Available at in.element14.com, in smd SOC package, 200 INR ](http://in.element14.com/microchip/mcp2515-e-so/can-controller-spi-10ma-18soic/dp/1605565)
	+ [Available at in.element14.com in Throgh hole, PDIP package, 155 INR](http://in.element14.com/microchip/mcp2515-i-p/controller-can-spi-pdip18-2515/dp/1439391)
+ MCP2551 CAN transceiver to give your board CAN-BUS capibility.
	+ [In DIP package, 101 INR](http://in.element14.com/microchip/mcp2551-e-p/ic-can-transceiver-dip8-2551/dp/1439745)
	+ [In SOC smd package, 107 INR](http://in.element14.com/microchip/mcp2551-e-sn/ic-transceiver-can-smd-8soic/dp/1467746)
+ [OpenSource schematics are here](http://www.seeedstudio.com/wiki/images/7/78/CAN-BUS_Shield_v0.9b.pdf)
+ Study is still on...
<br>
<hr>
<br>
### Mod Bus

+ Modbus is a serial communications protocol originally published by Modicon, now Schneider Electric, in 1979, for use with its programmable logic controllers. So this isn't any hardware, this is protocol which you can drive on RS232, RS485, even on CAN BUS, by writting the protocol on software part. This was developed for some important reasons in industry environment:

+ Developed with industrial application in mind
+ opnely published and rolyality free.
+ easy to deply and maintain.
+ moves raw bits or words without placing many restrictions on vendors.

+ Modbus enables communications between many devices, approx 240, connected on same network, for examplee a system that measures temperature and humidity and communicates the results to a computer, Modbus is often used to connect a supervisory computer with a remote terminal unit ( RTU ) in supervisory control and data acqusition systems ( SCADA ).

+ But there are some limitations, you can study about it, [here](http://en.wikipedia.org/wiki/Modbus)
+ There are modes under Modbus communication.
+ Please check here for your [FAQs regarding Modbus](http://www.simplymodbus.ca/FAQ.htm)
+ ModBus is a serial communication protocol. 
+ The device requesting the information is called the Modbus Master and the device supplying information are Modbus Slaves.
+ In standard network, there is one Master and upto 247 Slaves, each with a unique Slave address from 1 to 247. The Master can also write information to slaves.
+ official Modbus specification can be found at [www.modbus-ida.org](http://www.modbus-ida.org)
+ Modbus is an open protocol, meaning that it's free for manufacturers to build into their equipment without having to pay royalties. It has become a standard communications protocol in industry, and is now the most commonly available means of connecting industrial electronic devices. It is used widely by many manufacturers throughout many industries. Modbus is typically used to transmit signals from instrumentation and control devices back to a main controller or data gathering system, for example a system that measures temperature and humidity and communicates the results to a computer. Modbus is often used to connect a supervisory computer with a remote terminal unit (RTU) in supervisory control and data acquisition (SCADA) systems. Versions of the Modbus protocol exist for serial lines (Modbus RTU and Modbus ASCII) and for Ethernet (Modbus TCP).
+ Serial lines, or say modbus communication modes, RTU and ASCII mode of communication.
+ this can be implemented also on ethernet, Modbus on TCP.

+ [Arduino with modbus communication](http://playground.arduino.cc/Code/ModbusMaster), network connected from RS232, RS485 to try this library.
+ implementation of modbus on RS232, RS485, [please take a look here](http://www.rtaautomation.com/modbusrtu/).

+ Wires for modbus, people are using wires like telephone wires, like RJ11, RJ45 with less wires conncted for ethernet connection, and for RS232 connection/ network, RS232 cables are been used.

+ more is coming on this subject, regarding connectors and pin connections.


One thing you can take from this content is, Modbus is protocol that you can implement on various physical layers.
Plysical layers like RS232, RS422, RS485 and so on.
<br>
<hr>
Mail to: [Annim Banerjee](mailto:pixma38@gmail.com), [Alternate mail](mailto:annimbanerjee@nokiamail.com).
<hr>



