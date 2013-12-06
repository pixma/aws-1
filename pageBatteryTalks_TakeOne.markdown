---
title: pageBatterTalks
layout: default
---
# Data Logger with Low power.

## Lets collect the information about the components required for making data logger.

- Atmega328.
- Display.
- GSM.
- SD card.
- Battery.

## Lets note down the DC ratings of the above components.

- Atmega328
	- Running @ 1MHz 1.8 v draws 0.1uA in Power down mode.
- Display, JHD162A Display LCD 16 x 2
	- Volatge @ 3V consumes 0.2 uA.
	- Why not any other LCD.
	- WE have before us digit LCD.
	- 3- 1/2 Digit LCD. But these LCD are static.
	- Needs more IO pins.
	- Case with JHD162 and JHD204 have inbuild controller and power consumption is in mA units. Eliminate backlight.
- GSM at sleep mode state
	- at 3.1v 1.5 mA.
- SD card at 3.3 v
	- Current consumes 10 uA per pin .i.e. 3 pin equals 30 uA.
- Battery
	- AA+ 1.5 v , with 3 battery in series gives 4.5 v @ 2700mAH.
	- Shelf time is 10 years.
	- Internal resistance 150 milliohms

## Lets do calculations

- Lets add values
	- Atmega 0.1 uA.
	- Display 0.2uA.
	- GSM    1.5 mA.
	- SD card 30 uA.
	- Total = 1.5303 mA.
	- total ~ 1.55 mA.

- Battery life
	- 2700 mAH.
	- 2700 / 1.55  H = 1741.94 H
	- 1741.94 H / 24 = 72.58 Days
	- 72.58 / 30 days= 2.42 Months.

- With another Battery configurations
	- 2700 mAh * 2 = 5400mAh.( current capacity is been increased. )
	- 1.5 v * 4 ( 2 in series and 2 in parallel ) - 3.0 V
	- .i.e. AA Battery with 5400mAh with 4 pieces.
	- Total estimated current Consumption ~ 1.55 mA.
	- 5400 / 1.55 H = 3483.87 H.
	- 3483.87 / 24 day = 145.16 days.
	- 145.16 / 30 month = 4.8 months
So these are some calculations with battery with considering components are in stand by mode.
<br>
<hr>
## Doing the same calculations with taking 6 v 4.5 A Lead Acid battery( The last option )

- no carrying the same figures with Lead acid battery of 6V
- this will be last option to go with. 
<br>
<br>
<hr>

Email me at <a href="mailto:pixma38@gmail.com" > Annim Banerjee </a>
<br>
<hr>
