# Authos
![alt text](https://github.com/spezialis/authos/blob/master/readme_data/NEXT_AUTHOS_2017.gif)

[Lumères Festival 2017](http://www.festivallausannelumieres.ch/)

# Hardware
## LEDs Instructions
![](https://cdn-learn.adafruit.com/assets/assets/000/021/922/medium800/leds_dotstar-banner.jpg?1419375063)

- [Adafruit DotStar LEDs](https://learn.adafruit.com/adafruit-dotstar-leds)
- [Überguide](https://learn.adafruit.com/adafruit-neopixel-uberguide/the-magic-of-neopixels)

## Technical details
**Adafruit DotStar Digital LED Strip - 30 LED per Meter**
![alt text](https://github.com/spezialis/authos/blob/master/readme_data/2237-08.jpg)

### Technical specs
- Width (with weatherstripping): 14mm / 0.55"
- Width (w/o weatherstripping): 10mm / 0.4"
- Thickness (with weatherstripping):  4mm / 0.16"
30 LEDs per meter
- Pixel pitch: 33.3mm / 1.3" between LEDs

## Parts and Tools
### Parts
- Arduino UNO or Mega
- Stranded silicone-cover wire
- Heat shrink tubing
- Black adhesive tape

### Tools
- Hot Air Heat Shrinking
- Soldering station and accessories
	- Soldering iron
	- Soldering stand
	- Solder spool
	- Holder
	- Wire strippers
- Computer

### To Buy
- [ ] [Adafruit DotStar Digital LED Strip - Black 30 LED - Per Meter - BLACK](https://www.adafruit.com/product/2237)
- [ ] [4-pin JST SM Plug + Receptacle Cable Set](http://www.robotshop.com/en/4-pin-jst-sm-cable-set.html)
- [ ] [Female Dc Power Adapter - 2.1Mm Jack To Screw Terminal Block](https://www.adafruit.com/product/368)
- [ ] [5V 10A Switching Power Supply](https://www.adafruit.com/product/658)

## Important
### Distributing Power
For long strips, try to add a power tap every meter or so. This prevents a brown-out effect toward the end of the strip.

![](https://cdn-learn.adafruit.com/assets/assets/000/010/716/medium800/leds_nobrown.jpg?1377911872)

For best color consistency, aim for 1 meter or less distance from any pixel to a power connection. With larger NeoPixel setups, think of power distribution as branches of a tree rather than one continuous line.

### Estimating Power Requirements
To estimate power supply needs, multiply the number of pixels by 20, then divide the result by 1,000 for the “rule of thumb” power supply rating in Amps. Or use 60 (instead of 20) if you want to guarantee an absolute margin of safety for all situations. For example:

60 NeoPixels × 20 mA ÷ 1,000 = 1.2 Amps minimum<br>
60 NeoPixels × 60 mA ÷ 1,000 = 3.6 Amps minimum

## Maybe
Add a
- [PIR motion sensor](https://learn.adafruit.com/pir-passive-infrared-proximity-motion-sensor/overview) or
- [X-Band motion detector](https://www.parallax.com/product/32213) or
- ...
to activate the vitrine when someone is near it.

# Credits
AUTHOS<br>
Stella + Arthur + Alexander
