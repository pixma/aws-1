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
+ MOD Bus

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
<hr>

### Mod Bus

<br>
<hr>
Mail to: [Annim Banerjee](mailto:pixma38@gmail.com), [Alternate mail](mailto:annimbanerjee@nokiamail.com).
<hr>



