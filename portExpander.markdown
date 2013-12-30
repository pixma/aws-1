---
title: port Expander 
layout: default
---

## Port expansion

People are expanding thier general purpose IO ports based on some protocols
- I2C Bus interface.
- SPI interfacing.
<br>
<hr>
<br>
### Port expander ICs are used frequently used, companies are
- Philips, PCF8574
- Maxim
- Microchip

<br>
<hr>
<br>
### From philiphs, [Tutotial from here](http://playground.arduino.cc//Main/PCF8574Class)

#### Intro

The I2C bus can be used to extend the number of IO lines. A frequently used chip for this is the PCF8574 which offers 8 IO lines. The PCF8474 has multiple address lines so the I2C address can be changed. 

Features
- Operating Voltage 2.5v to 6v.
- Low stand by current of 10uA maximum.
- I2C bus to parallel port expander.
- 16 addressable individual IO pins.
- Package available in DIP24.
- This ic remains simple device.
- This is bi directional.
- Two Port is been provided by this IC.
- [Vendor Availability](http://www.protocentral.com/prototyping/137-breakout-board-for-pcf8575-i2c-expander.html)
- [From element14 india](http://in.element14.com/jsp/search/browse.jsp?N=2103+203654&Ntk=gensearch&Ntt=PCF8574&Ntx=mode+matchallpartial)
- [Detailed datasheet from TI](http://www.ti.com/lit/ds/symlink/pcf8575c.pdf)
- [Examples are available for AVR and mbedded too](http://www.protocentral.com/prototyping/137-breakout-board-for-pcf8575-i2c-expander.html).
- Block Diagram shown below 
<br>

![alt text](./images/pcf8575_blockDiag.png)

<br>
- Pin configuration of DIP package
<br>
![alt text](./images/pcf8575_PinConfig.png")

<br>
- Profit of using this : we will get 2, 8 bit digital, bi directional port, on I2C bus.
<br>
<hr>
<br>
### From microchip [Please check here](http://tronixstuff.com/2011/08/26/tutorial-maximising-your-arduinos-io-ports/)
<br>
#### INTRO
<br>
- The Microchip MCP23017 16-bit serial expander with I2C serial interface. This 28-pin IC offers sixteen inputs or outputs – and up to eight of the ICs can be used on one I2C bus… offering a maximum of 128 extra I/O ports.                                             
<br>
Features
<br>
- Operating Voltage 1.8v to 5.5v
- Low stand by current 1uAmax.
- Three hardware address pins to allow up to eight devices on the bus.
- High SPEED SPI interface. Upto 100 MHz.
- HIGH SPEED I2C interface. Upto 1.7 MHz.
- 16 bit bi directional IO port.
- IO ports are input by default.
- 28 pin DIP package.
- Configurable interrupt output pins
- Configurable as active-high, active-low or open-drain
- INTA and INTB can be configured to operate independently or together.
- Block diagram is shown below
<br>
![alt text](./images/mcp23017_blockDiagram.png)
<br>
- Pin Configuration of the same
<br>
![alt text](./images/pinConfig_mcp23017.png)
<br>
- [Example with arduino](http://tronixstuff.com/2011/08/26/tutorial-maximising-your-arduinos-io-ports/).
- [sunrom technology, with interfacing schematic](http://www.sunrom.com/445)
- [Vendor availability in ebay india](http://www.ebay.in/itm/Simple-cheap-I-O-expansion-Microchip-MCP23017-Raspberry-Pi-Arduino-/271296353852).
- [in.element14 vendor](http://in.element14.com/microchip/mcp23017-e-so/i-o-expander-ic/dp/1262563).
- Advantage to use this is , we will have 2 ports from this IC.
- I2C and SPI interfacing mode with fast communication speed.
- Interrupt logic available.
- Parallel IO expansion with I2C or SPI interfacing.
- Configurable to operate as 8 bit or 16 bit IO port.
- This 28-pin IC offers sixteen inputs or outputs – and up to eight of the ICs can be used on one I2C bus… offering a maximum of 128 extra I/O ports.
<br>
<hr>
<br>
### Comparision table based on some parameters

![alt text](./images/table.png)
<br>
<hr>
<br>
### What more can be done around the way
- [Expanding the arduino, the cheapest way around](http://www.thekanes.org/2010/06/09/expanding-the-arduino-cheap-ways-to-add-output-pins-and-power/)
- [Hack a day , simple pin expansion with user comments underneath](http://hackaday.com/2011/11/08/a-simple-method-for-expanding-arduino-io-capacity/)
- [expand-io-ports-with-another-arduino, with sample code](http://rodelectronics.blogspot.in/2010/03/expand-io-ports-with-another-arduino.html)
- [arduino nxp port expander examples giving](http://playground.arduino.cc/Code/I2CPortExpander8574)
<br>
<hr>
[Annim Banerjee](mailto:pixma38@gmail.com)
<hr>
