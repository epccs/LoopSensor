# Moisture and Temperature Sensor

![Status](https://raw.githubusercontent.com/epccs/LoopSensor/master/MT/status_icon.png "MT Status")

Acts as a capacitive soil moisture sensor.

## Overview

It is mostly the water content that changes the capacitance. The dielectric constant of water also varies with temperature, so that needs to be taken into account.

https://nvlpubs.nist.gov/nistpubs/jres/56/jresv56n1p1_A1b.pdf

Some years back, I tinkered with this CMOS 555 timer set up that oscillats as a function of the sensor capacitance. I used a CAT5 pair as the soil moisture sensor. Used current mirrors and voltage references to make the oscillator ramp reasonably linear (the idea is to keep the math simple). The oscillator turns on and off a current source so that I can transmit the oscillation events over a current loop (another CAT5 pair) to input capture hardware on an AVR. I added a thermistor so that the ratio of the high side of the pulse to the low side tells the thermistor value (and that tells the temperature). Making sense of the data is a problem I have yet to overcome, I need to compensate (the capacitive measurement) for the effect of temperature on the dielectric constant, and calibrate it with the porous encasing I used.

![Schematic](https://raw.githubusercontent.com/epccs/LoopSensor/master/MT/16052,Schematic.png "MT Schematic")

![Bottom](https://raw.githubusercontent.com/epccs/LoopSensor/master/MT/16052,Bottom.png "MT Board Bottom")

![Top](https://raw.githubusercontent.com/epccs/LoopSensor/master/MT/16052,Top.png "MT Board Top")