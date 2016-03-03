# 230 / 110 V~ Heated Bed
A mains voltage heated bed that outputs 500 W of heat (2 minutes heatup time to 110 °C), works for 230 V~ and 110 V~ and also features the good old power status LED.

![render of top](https://cdn.hackaday.io/images/7579811449431756922.png)
![render of bottom side](https://cdn.hackaday.io/images/5494491449432442830.png)

## Caution
- this is highly experimental
- do not use this if you don't know what you're doing
- don't hold me responsible for the outcome of what you do with the information in this repository
- even if operated electrically correct this device is dangerous and can get hot enough to seriously injure humans and animals.

## Project status and compatibility
- [x] layoutet v01
- [x] compatible to MK2/B heated bed in terms of dimensions / mounting hole spacing
- [x] compatible to most MK2/B heated beds in terms of endstop position
- [x] added 110 and 230 V~ compatibility by wiring options
- [x] added thermal fuse
- [x] added LED overcurrent fuse
- [x] added warnings, wiring and instructions to the silkscreen
- [ ] not tested
- [ ] cannot be considered safe yet
- [ ] milled polycarbonat led/fuse cover is in preparation but not yet done

## Specifications
- Power consumption:	500 W (230 V~) or 460 (110 V~)
- Operation Voltages:	230 V~ (110 V~ over a center tap)
- Resistance:	~106 Ω
- Trace length: about 402 x 200 mm = ~80,800 mm
- Copper thickness (on PCB):	1oz aka 1.37 mil aka 35 µm
- Trace width:	0.37 mm
- Safety features: fused power indicator LED with protective polycarbonat cover, thermal fuse

## How to use
Know what you do. Solder components as described in the BOM, make sure no excess solder can cause shorts of any kind. Wire as instructed on the backside of the PCB, do not use without professional supervision and appropriate safety precautions. Do not use without closed loop temperature control, i.e. with a thermistor/thermocouple and SSR, since the thermal fuse is supposedly a safety feature rather than a means of temperature control.

## Why?
There are many benefits of a mains voltage PCB heated bed: I will be driven directly from mains, skips the need for an expensive power supply, high current heatsinked SSR and heavy wire. Instead, it can be driven by a cheap low current SSR without heatsink. It's also cheaper to manufacture and provides more structural support for your printing plate than silicone heater pads.
IMHO, it’s pretty much nuts to convert down mains voltage in a power supply to 12/24V just to drive a heating element, except that it „feels“ a bit safer. Also, it’s a false assumption, that a 12/24 V heated bed is actually safe, since in case of an unexpected malfunction it will still burn down your place - regardless of the voltage on the heating element. Using fuses, temperature feedback and considering failure scenarios cannot be omitted anyway.

## Disclaimer
I am not responsible for the outcome of what you do with this information. As said, this is a highly experimental and untested prototype.

## License
Created by Moritz Walter 2015, released under [CC-BY-NC-SA](http://creativecommons.org/licenses/by-nc-sa/3.0/legalcode)
