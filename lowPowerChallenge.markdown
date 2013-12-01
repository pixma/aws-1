---
title: LowPowerBoards
Layout: default
---

## Low power Challenge
<hr>
 + To run our system for long time such as 3-5 years without touching the power sources whatever they are.
 #### Power sources options before us are-
 + Battery
	- Alkaline.
	- AA+ - Ni-MH.
	- AAA  Battery.
	- Lipo Battery.
	- Li-ion Battery.
	- Lead Acid Battery.
+ Solar
	- Solar panel as power source.
+ To run any digital system for so long, what factors should support 
	+ Battery or say power source self-discharge rate should be as low as possible.
	+ Current consumption by the digital system should be as much low as possible.
	+ Let digital system should use power only when required.
	+ Use low power or ultra-low power components on circuit.
	+ Place lesser components on board so only essential components will draw current.
<hr>

+ Lets go for some calculations 
	+ consider for 3 years.
	+ which is equals to 3 x 365 x 24 = 26289 Hrs.
	+ consider AA+ battery with current capacity of 2500mAH, rechargable battery suppose.
	+ Slef Discharge rate: 2 - 3 percentage, per month. That is, by self discharging rate of 2 percentage, battery discharge by 50 mA per month.
	+ Scenario :-
	+ Net Current consumption by digital system if kept lower than self dischargeing rate then 
	consider these calculations again:
	+ Suppose Net current consumption is 30mA.
	+ This battery will run for 2500mA / 30 mA is equals to 83.3 Hrs.
	+ Recharge the battery as it reaches down by 10 percent.
	+ Then again it runs for 83.3 Hrs.
	+ This makes 26289 / 83.3 Hrs equals to 316 times recharging.
	+ Also, battery also takes time for charging and at same time it also powers up the digital system.
	+ Above calculation is based on ideal conditions.
<hr>

### From above calculations, 

+ We need to detect battery voltage level.
+ We need to protect from over charging and also avoid under charging.

<hr>

## Low, ultra low power components

+ Microcontroller
+ Sensors
+ GSM


<hr>


