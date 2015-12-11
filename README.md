# 230 / 110 V~ Heated Bed
A mains voltage heated bed that outputs 500 W of heat (3 minutes heatup time to 110 °C), works for 230 V~ and 110 V~ and also features the good old power status LED.
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
- [x] added led overcurrent fuse
- [x] added warnings, wiring and instructions to the silkscreen
- [ ] not tested
- [ ] cannot be considered safe yet
- [ ] milled polycarbonat led/fuse cover is in preparation but not yet done

## How to use
Know what you do. Solder components as described in the BOM, make sure no excess solder can cause shorts of any kind. Wire as instructed on the backside of the PCB, do not use without professional supervision and appropriate safety precautions. Do not use without closed loop temperature control, i.e. with a thermistor/thermocouple and SSR, since the thermal fuse is supposedly a safety feature rather than a means of temperature control.

## Disclaimer
I am not responsible for the outcome of what you do with this information. As said, this is a highly experimental and untested prototype.

## License
I've not yet chosen a license for this yet, please ask if you want to redistribute this or wait until license has been determined. Created and copyrighted by Moritz Walter 2015