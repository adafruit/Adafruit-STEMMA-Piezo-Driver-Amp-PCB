## Adafruit STEMMA Piezo Driver Amp - PAM8904 PCB

<a href="http://www.adafruit.com/products/5791"><img src="assets/5791.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit STEMMA Piezo Driver Amp - PAM8904. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5791

### Description

Piezos make noise when you put an AC voltage across them: and the bigger the Vpp the louder they are. With your standard 3V logic microcontroller you can make 3Vpp with a PWM out, or 6Vpp differential with two complimentary outputs. But what if you want even louder? Or if you're using a piezo to sense distance using ultrasonic bounces?

We found the nifty PAM8904, which is an amplifier specifically designed for driving piezo elements - and unlike audio amplifiers it's good for up to 300 KHz! It's a switched-cap piezo driver that has bridge-tied load (BTL) output and up to 3x voltage multiplication thanks to a built in boosting circuit for up to ~13Vpp.

We whipped up a quick breakout in our 2mm JST-PH STEMMA form-factor to make it easy for anyone who wants to beep their boops very loudly. 

Usage is easy: power with 3 to 5VDC on the Vin and GND pins. Then provide a square wave on the signal pin, from 20Hz to 300KHz - any duty cycle is ok but 50% will probably work best. Theres a dual DIP switch to set the gain: you can set it to off (zero gain), x1 gain, x2 gain and x3 gain. The output is differential so 2x gain will give you 4xVin peak-to-peak across the piezo lines. Connect your piezo to the terminal block and you're ready to rock. 

Please note: If you are powering the driver from 5VDC, don't set the gain to x3 because the 15V output is higher than the driver is specified for. (Yeah we also sorta wondered why the chip manufacturer allows it). So if you are using 3.3V power, x3 gain is OK and will give you about 10V out but if you're powering with 5V use 2x gain max to keep the max voltage at 10V.

Piezo element and 3-pin JST PH cable not included! But we stock em in the shop if you want to pick up separately.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
