# LoRa-GateWay
LoRa GateWay
*** IMPORTANT ***



Single Channel LoRaWAN Gateway
This repository contains a proof-of-concept implementation of a single channel LoRaWAN gateway.

It has been tested on the Raspberry Pi platform, using a Semtech SX1272 transceiver (HopeRF RFM92W), and SX1276 (HopeRF RFM95W).

The code is for testing and development purposes only, and is not meant for production usage.

Part of the source has been copied from the Semtech Packet Forwarder (with permission).


Dependencies
SPI needs to be enabled on the Raspberry Pi (use raspi-config)
WiringPi: a GPIO access library written in C for the BCM2835 used in the Raspberry Pi. sudo apt-get install wiringpi see 

Connections
SX1272 - Raspberry

3.3V - 3.3V (header pin #1) GND	- GND (pin #6) MISO - MISO (pin #21) MOSI - MOSI (pin #19) SCK - CLK (pin #23) NSS - GPIO6 (pin #22) DIO0 - GPIO7 (pin #7) RST - GPIO0 (pin #11)

Configuration
Defaults:

LoRa: SF7 at 868.1 Mhz
Server: 54.229.214.112, port 1700 (The Things Network: croft.thethings.girovito.nl)
Edit source node (main.cpp) to change configuration (look for: "Configure these values!").

Please set location, email and description.


