# Pedal Lighting Remix
This work is based on the work done by [Pedal Lighting team](https://www.petallighting.com/)

# The Controller
The soon to be designed controller.
The controller designed for the project is good - [Dig-Octa](https://quinled.info/quinled-dig-octa/)

But I have a few things I want to do differently.

## What am I building?
- ESP32S3 MCU
- 4 neopixel lines
- Using Speakon 4 pole connectors for the fixture
- Adding RS485 for the fixture signalling
- Adding power protection for the fixtures
  * Poly fuses per fixture (resettable fuse)
  * TVS diode (protect from power spikes)
  * Bulk capacitor (protect from hot plugging)
- Data line protection
  * adding RC circuit that will temporarly stop data slow when plugging / unplugging fixtures
- Adding Ethernet support
- Will have two rs485 modules
  * can be used for RS485 or DMX
  * can be used as input or output
- Support DMX over ESPNOW
- Adding QWIIC I2C connectors for expanable modules