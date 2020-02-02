# Automatic Cheese Maker

## Intro
The Automatic Cheese Maker (ACM) is a tool to reduce the effort of making cheese, it has the following features:

- Heater (via a water bath)
- Stirrer (via a 3d printed stirrer and stepper)
- Ingredient releaser tool (via egg cups and servos)

It reduces the initial effort for making cheese but does not do all of the job. The following are not performed by the ACM and have to be done by hand still:

- Curd Cutting
- Draining
- Pressing
- Etc

## Pictures

## Parts

### WaterBath
The WaterBath part of the ACM is made using a similar method to a [brew kettle instructable](https://www.instructables.com/id/Build-Your-Own-Brewery-for-Under-100-STEP-2-/). You will need the following parts:

- [£6 Wilko kettle](https://www.wilko.com/en-uk/wilko-white-cordless-17l-kettle/p/0316169)
- [£20 Wilko 12L StockPot](https://www.wilko.com/en-uk/wilko-stock-pot-12l/p/0322498)
- [£26 21L StockPot](https://www.amazon.co.uk/gp/product/B07B9F4D6Q)
  - The above 21L StockPot has the following size: diameter 30 cm, height 30 cm
- [£4 DS18B20 Waterproof Digital Probe](https://www.ebay.co.uk/itm/DS18B20-Waterproof-Digital-Probe-Temperature-Sensor-Silicone-Cable-Thermometer/332222916282)
- [£4 1/2"NPT Thermowell 50mm length](https://www.ebay.co.uk/itm/Stainless-Steel-Thermowell-1-2-NPT-Threads-50-250-Temperature-Sensor-UULK-/264221201183)

You will also need to print the [KettleElementCap](https://github.com/AutomaticCheeseMaker/CheeseMaker-3DParts)

### Stirrer/Ingredient releaser
The Stirrer part of the ACM is the 3D printed bit that sits on top of the pot and stirs and releases ingredients. The following parts are needed:

- [£4 DS18B20 Waterproof Digital Probe](https://www.ebay.co.uk/itm/DS18B20-Waterproof-Digital-Probe-Temperature-Sensor-Silicone-Cable-Thermometer/332222916282)
- £4 1/2"NPT Thermowell 250mm length
- £8 Nema 17 1.8° Stepper Motor
- £12 4x Tower Pro SG-90 SG90 9g Micro Servo
- [£6 4x Egg Cups](https://www.amazon.co.uk/gp/product/B001CN0S38/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)

You will also need to print [StirrerArm and StirrerHolder](https://github.com/AutomaticCheeseMaker/CheeseMaker-3DParts)

### Control Circuit
The software runs on an Arduino Mega and a machine capable of running OctoPrint (this could be a raspberry PI or a PC).

The software stack consists of:
- [OctoPrint/OctoPi](https://octoprint.org/)
- [OctoCheese Plugin](https://github.com/AutomaticCheeseMaker/OctoCheese)
- [Custom Marlin Firmware](https://github.com/AutomaticCheeseMaker/Marlin)

The hardware stack consists of:
- £8 Arduino Mega 2560
- [£20 Custom Circuit Board + Components](https://github.com/AutomaticCheeseMaker/CheeseMaker-Circuit)
- £5 Solid State Relay 220V AC Output, 5V DC Input
- [IEC C15 Orange 3m Cable](https://www.ebay.co.uk/itm/Power-Extension-Cable-IEC-C14-Male-Plug-IEC-C15-Female-Socket-3m-3metre-ORANGE/202315430599)

You will also need to print [HardwareCase](https://github.com/AutomaticCheeseMaker/CheeseMaker-3DParts)
