# Authos
![](https://github.com/spezialis/authos/blob/master/readme_data/NEXT_AUTHOS_2017.gif)

[Lumères Festival 2017](http://www.festivallausannelumieres.ch/)

## Parts and Tools
### Parts I
- Arduino UNO
- Stranded silicone-cover wire
- Heat shrink tubing
- Colored adhesive tape

### Parts II
- 557 LEDs
- 32 strips cuts
	- 6 strips cuts for distributing the power

### Tools
- Hot Air Heat Shrinking
- Soldering station and accessories
	- Soldering iron
	- Soldering stand
	- Solder spool
	- Holder
- Wire strippers
- Computer

# Hardware
## Timer
Night ON illumination and day OFF

![](https://s3.amazonaws.com/learn-production/guides/images/000/001/231/medium800/thump.jpg?1454534952)

- [Adafruit DS1307 Real Time Clock](https://learn.adafruit.com/ds1307-real-time-clock-breakout-board-kit/assembly?view=all)
- [Arduino Time library](https://playground.arduino.cc/Code/Time)
- [RTC library](https://github.com/adafruit/RTClib)

#### Arduino UNO-to-RTC connections
The board must be connected to the "in" end of the LED strip.  Data flows one way through the strip, from "in" to "out".

| Arduino  	| DotStar 			|
| --				|	-- 						|
| A5 				| SCL					 	|
| A4  			| SDA						|
| + or 5V  	| + or 5V  			|
| GND  			| GND 					|

## LEDs Instructions
![](https://cdn-learn.adafruit.com/assets/assets/000/021/922/medium800/leds_dotstar-banner.jpg?1419375063)

- [Adafruit DotStar LEDs](https://learn.adafruit.com/adafruit-dotstar-leds)
- [Überguide](https://learn.adafruit.com/adafruit-neopixel-uberguide/the-magic-of-neopixels)

### Technical details
**Adafruit DotStar Digital LED Strip - 30 LED per Meter**
![alt text](https://github.com/spezialis/authos/blob/master/readme_data/2237-08.jpg)

#### Technical specs
- Width (with weatherstripping): 14mm / 0.55"
- Width (w/o weatherstripping): 10mm / 0.4"
- Thickness (with weatherstripping):  4mm / 0.16"
30 LEDs per meter
- Pixel pitch: 33.3mm / 1.3" between LEDs

### To Buy
- [x] [Adafruit DotStar Digital LED Strip - Black 30 LED - Per Meter - BLACK](https://www.adafruit.com/product/2237) x 20
- [ ] [4-pin JST SM Plug + Receptacle Cable Set](https://www.amazon.de/gp/product/B01D9JD4ZG/ref=ox_sc_act_title_1?smid=AGJ2TI2R2YFK8&psc=1) x 26
- [x] [2-pin JST SM Plug + Receptacle Cable Set](http://www.robotshop.com/en/2-pin-jst-sm-cable-set.html) x 12
- [x] [Female Dc Power Adapter - 2.1Mm Jack To Screw Terminal Block](https://www.adafruit.com/product/368) x 2
- [x] [5V 10A Switching Power Supply](https://www.adafruit.com/product/658) x 2
- [ ] capacitor (1000 µF, 6.3V or higher) x 2
- [ ] [Adafruit DS1307 Real Time Clock](https://www.adafruit.com/product/3296#tutorials) x 2

### Important
#### Distributing Power
For long strips, try to add a power tap every meter or so. This prevents a brown-out effect toward the end of the strip.

![](https://cdn-learn.adafruit.com/assets/assets/000/010/716/medium800/leds_nobrown.jpg?1377911872)
![](https://github.com/spezialis/authos/blob/master/readme_data/Led_power.png)

For best color consistency, aim for 1 meter or less distance from any pixel to a power connection. With larger NeoPixel setups, think of power distribution as branches of a tree rather than one continuous line.

#### Estimating Power Requirements
To estimate power supply needs, multiply the number of pixels by 20, then divide the result by 1,000 for the “rule of thumb” power supply rating in Amps. Or use 60 (instead of 20) if you want to guarantee an absolute margin of safety for all situations. For example:

60 NeoPixels × 20 mA ÷ 1,000 = 1.2 Amps minimum<br>
60 NeoPixels × 60 mA ÷ 1,000 = 3.6 Amps minimum

#### Board-to-DotStar connections
The board must be connected to the "in" end of the LED strip.  Data flows one way through the strip, from "in" to "out".

| Arduino  	| DotStar 			|
| --				|	-- 						|
| 11 				| DI (Data In) 	|
| 13  			| CI (Clock In) |
| + or 5V  	| + or 5V  			|
| GND  			| GND 					|

#### DotStar-to-Power connections
The power supply will be connected in the middle of the strip. Putting it in the middle will minimize the number of pixels the power needs to flow through.

| LED Strip "out" connector | LED Strip "in" connector |
| -- 												| -- 											 |
| LED Strip + Wire  				| Screw Terminal +  			 |
| LED Strip - Wire 					| Screw Terminal -  			 |

![](https://learn.adafruit.com/assets/45036)
![](https://learn.adafruit.com/assets/45037)

#### References
Check also this links:
- [Dotstar LED](https://learn.adafruit.com/neopixel-and-glass-pebble-floor/neopixel-assembly?view=all#step-2)
- [Creating FastLED Color Palettes](https://learn.adafruit.com/twinkling-led-parasol/assembly) x 2
- [FastLed Library](http://fastled.io/)
- [FastLed Library Github](https://github.com/FastLED/FastLED)

## Maybe
Add a motion sensor to as an on/off switch and to start looping through animations:
- [PIR motion sensor](https://learn.adafruit.com/pir-passive-infrared-proximity-motion-sensor/overview) or
- [X-Band motion sensor](https://www.parallax.com/product/32213)

# Todo
- [x] Test the best distance between the LED and the window (Use some semi-transparent paper)

# Credits
AUTHOS<br>
Stella + Arthur + Alexander
