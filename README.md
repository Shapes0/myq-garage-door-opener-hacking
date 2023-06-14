# myq-garage-door-opener-hacking
Research to hopefully liberate my myQ garage door opener from "the cloud"

## Specs
|Type|Description|
|-|-|
|Wi-Fi Module|WM-N-BM-14|
|SoC|STM32F205RGY6|
|FCC ID|https://fccid.io/HBW1D8088-1|

## Possibilities
There is a IoT specific module from particle.io called the [Particle P1](https://docs.particle.io/reference/datasheets/wi-fi/p1-datasheet/). It seems to be nearly identical to the WM-N-BM-14, carrying a WM-N-BM-14-S. This connects to their cloud, but we can [self host](https://github.com/Brewskey/spark-server) the API server and keep the communication local. If we were to solder this module in and reverse the internal I/O communication, then we can control the device locally.

## Path forward
This is about as far as I know how to get, does anyone with more experience find this useful?
