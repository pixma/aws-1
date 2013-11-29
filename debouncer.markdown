---
title: debouncer
layout: default
---
## Debouncer
<hr>
<br>
###Debouncer IC using
+ MC14490 IC
	+ [Datasheet](http://www.onsemi.com/pub_link/Collateral/MC14490-D.PDF)
	+ Six Debouncers in one package.
	+ TTL compatible.
+ The MC14490 is constructed with complementary MOS enhancement mode devices, and is used for the elimination of extraneous level changes that result when interfacing with mechanical contacts.

+ pin configuration

<center>
<img src="http://www.labbookpages.co.uk/electronics/files/debounce/MC14490.png" width="300" height="300" />
</center>
<br>
+ Sample connection with button and an led, please reffer the pin assignment diagram to understand the connections.

<center>
<img src="images/mc14490_interface.png" width="550" height="400" />
</center>
<br>
+ Calculations
<br>
	`T = 2.67 * C , C in nF.T = time.C = capacitor in nF unit.`
<br>
<br>
+ Thus from the above equation, we can calculate capacitor value for achieving desired clocks.
+ Now, MC14490 smoothens the output signal.
+ For 10nF capacitor, we get ~26msecs 0f clock.

<hr>
### Current Consumption 
##### Ratings
<br>

+ Supply Voltage range: -0.5v to 18.0 v.
+ Power Dissipation, per package: 500 mW.
+ Input current per pin: +- 10 mA.
+ internal Diode protection in all IO pins.
<br>
<br>

We also have to minimize the current consumption in this IC. We can give as low as 1 v to this IC but e have to put ~10mA on IO pin for getting good results from MC14490.


<hr>
<br>
<br>
Your comments are welcome.
<br>
Mail me at <a href="mailto:pixma38@gmail.com"> Annim Banerjee </a>
<br>
<hr>

