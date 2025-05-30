---
title: Other Hardware
hide:
  # - navigation
  # - toc
---

!!! note ""
    Still under construction, feel free to add to the list!

This page lists some third-party hardware and/or tools that are working with WLED!

Please use a decent and neutral description when adding things to this list.

!!! tip
    Lists are in alphabetical order. The position of an item in the list does not indicate how good it is or if it will fit your use case.
    Please carefully compare all items in the category you are interested in, and you should find the one that suits your needs best in just a few minutes! 

## Addressable LED Strips

Sorting: 5v data only, 5v Data + Clock, 12v data only

| Type | Voltage | Comments |
|---|---|---|
SK6812 | 5v/12v | RGBW
WS2811 | 5v | usually found in IP68 sealed 12mm pixel strings
WS2812B | 5v |
WS2813 | 5v | has a backup data line
APA102 | 5v | using 2 data pins, Clock and Data
LPD8806 | 5v | using 2 data pins, Clock and Data
WS2801 | 5v | using 2 data pins, Clock and Data
SK9822 | 5v | using 2 data pins, Clock and Data
GS8208 | 12v |
TM1814 | 12v | RGBW
WS2811 | 12v | usually 3-LED segments, has data-line resistor
WS2815 | 12v | has a backup data line

## Non-Addressable LED Strips

WLED supports non-addressable LED strips as well. Unlike addressable strips, non-addressable strips require a pin for each "color" channel. To drive these strips, additional circuits (MOSFETs) are required.
As of v0.13.1, WLED supports single color, CCT, RGB, RGBW and RGBCCT strips. These strips are commonly found at 12 or 24 volts.
The default PWM frequency for dimming is 880 Hz on ESP8266 and 19531 Hz for ESP32.

## Controllers with WLED pre-installed

!!! check "Info"
    Unless otherwise noted, controllers feature everything you need for most WLED setups, except a power supply, wiring and fuses, and of course the LEDs themselves!
    
| Name | Description |
|---|---|
[8 Port LED Distro](https://www.tindie.com/products/bong69/8-port-led-distro/) | This is an 8 port ESP32 based LED distro board running WLED. Distributing both power and data in 1 board. The WT32-ETH01 provides support for Wi-Fi or ethernet connections. It can be used with either 5v or 12v or 24v LED pixels. Also includes a USB-C port for programming, level shifter, 5 amp fuse on every port, multiple voltage inputs with no jumpers to set and phoenix connectors for easy wiring.
[A1-SLWF-02 WLED controller](https://smartlight.me/led-strips/adressable-led-strips/controller-slwf-02) | WLED dedicatedly designed Controller that supports 5V-12V addressable strips from Ukrainian developers. Based on ESP8266. Slim design, sensor button, powered either by type-C or screw-terminal. Screwdriver included. [Worldwide delivery](https://smartlight.me/led-strips/adressable-led-strips/controller-slwf-02).
[ABC! WLED Controller / ESP8266](https://shop.myhome-control.de/ABC-WLED-Controller-V31-ESP8266/HW10002) | Commercial controller for 5V LED strips. Based on ESP8266 uC. Two outputs. Ready to use. Additional Relay&Fuse board available. (German shop & shipping only within Germany). A similar one is available at [WLED.SHOP](https://wled.shop/produkt/wladis-wled-controller-v31/)
[ABC! WLED Controller / ESP32](https://shop.myhome-control.de/ABC-WLED-Controller-V41-ESP32/HW10003.1) | Commercial controller for 5V LED strips. Based on ESP32 uC. Two outputs. Option for digital microphone / sound reactive. Ready to use. Additional Relay&Fuse board available. (German shop & shipping only within Germany). A similar one is available at [WLED.SHOP](https://wled.shop/produkt/wladis-wled-controller-v40-esp32/).
[ABC! WLED Shield, all-purpose, for ESP8266/ESP32](https://shop.myhome-control.de/ABC-WLED-Basis-Board-fuer-5V-und-12V-LED-universell/HW10008) | Commercial WLED Shield for 5V/12V LED strips. To be used with ESP8266 or ESP32 in D1 mini format. Two outputs. Option for digital microphone / sound reactive (with ESP32). Automatic 5V/12V recognition (no jumper/switch etc. required). Enclosure is available too. German shop & shipping currently only within Germany.
[Athom Light Strip Controller](https://www.aliexpress.com/item/1005002198527735.html) | Simple controller with enclosure for reliably driving 3 pin 5V LEDs. Uses 2M ESP8266.
[Athom High Power Addressable LED Strip Controller](https://www.athom.tech/blank-1/wled-high-power-led-strip-controller) | Higher power options than the above system. Supports optional clock output.
[Athom LS8P ESP32 Music Controller](https://www.athom.tech/blank-1/wled-esp32-music-addressable-led-strip-controller) | ESP32 based controller with dual output, microphone and IR. Comes with WLED preinstalled
[Athom RGBW Light Strip Controller](https://www.athom.tech/blank-1/wled-rgbw-light-strip-controller) | Has outputs for individual color channels.
[Cadsbi Motion Smart](https://www.cadsbi-shop.de/shop/led-beleuchtungscontroller/cadsbi-motion-smart/) | Ready to use solution with 3 output ports, an external antenna, in a high quality metal enclosure
[cod.m Wi-Fi Pixel Controller](https://shop.codm.de/automation/pixel/30/wlan-pixel-controller) | Fully completed control PCB with level shifter, terminals and case - pre-flashed with WLED!
[ESP8266 Pixel Controller](https://www.maltepoeggel.de/?site=pixelcontroller) | DIY board for 5V/12V LED strips with TTL or RS485 output using a Wemos D1 mini, integrated fuse, pluggable terminal block, 3D printed module case
[ESPthings.io ET-AL01](https://www.espthings.io/AL01) | DIY board for 5 Analog channels and/or up to 5 Digital LED channels (or a combination of the latter as required), Integrated level shifter, 5v/12/24v compatibility, 4x pull-up/down GPIO, serial interface and power distribution terminals. Can be used with Wemos D1-style ESP8266 or ESP32 boards.
[ESP32 WLED pico board](https://www.tindie.com/products/28276/) | ESP32 WLED pico board,super small form factor, ready to buy on [Tindie](https://www.tindie.com/products/28276/) and [Tindie EU](https://www.tindie.com/products/moonmodules/esp32-pico-board-with-digital-microphone/). Integrated level shifter, exposed pins for extending functionality , on board I2S microphone, [Firmware is here](https://github.com/srg74/WLED-ESP32-pico/tree/main/Firmware). Project page is [here](https://github.com/srg74/WLED-ESP32-pico)
[IOT4WLED](https://iot4.eu/product/iot4wled/) | Ready to use hardware for WLED!
[Laterna](https://github.com/Planet-Laterna/Laterna) | Based on an ESP32 for digital LED and RBG/RGBW LED strips with support for 5V, 12V and 24V LED strips. (Up to 4 channels)
[Laterna Mini V3](https://github.com/Planet-Laterna/Laterna-mini-V3) | Small ESP32 based controller with optional digital microphone integrated for digital 5V LED strips.
[Laterna Stick](https://github.com/Planet-Laterna/Laterna_Stick) | USB Stick like ESP32 based controller for digital 5V LED strips.
[LedBox V3](https://stanleyprojects.com/projects/ledbox_v3/) | LedBox V3 by StanleyProjects is the ultimate sound-reactive addressable LED controller powered by ESP32-S3. It is compatible with 5-12V addressable LED strips (WS281x, SK6812, etc.), supporting both 3(data) and 4(data,clock) wire signal protocols. It has a digital MEMS microphone, MOSFET, logic-level converter, button, IR demodulator, variable imedance-matching resistor, USB-C port, and a safety resettable fuse, all in a compact 3D printable case, and flashed with [WLED-MM](https://github.com/MoonModules/WLED). More information and purchase links are available [here](https://stanleyprojects.com/projects/ledbox_v3/).
[Luminxa v2.2.2](https://luminxa.com/product/luminxa-2-2-2/) | ESP32 | ESP32 Based board with 12 WS2812 LEDs Onboard (6 on each side) + Gyro Sensor (Business project)
[My Baby's Got LED](https://tindie.com/products/mcqn_ltd/my-babys-got-led/)| [Certified open hardware](https://certification.oshwa.org/uk000030.html). Easy plug-and-play WLED board for those that don't want to figure out the hardware - you won't even need a screwdriver to get started. PC power supply ([ATX](https://en.wikipedia.org/wiki/ATX#:~:text=An%20ATX%20power%20supply%20provides,the%20original%2020-pin%20version.)) powers three 5V injection points on 8A fuses. For sale now on [Tindie](https://tindie.com/products/mcqn_ltd/my-babys-got-led/)! Full details on [the github repo](https://github.com/mcqn/my-babys-got-led) and [maker's website](https://mcqn.com/ibal223/).
[QuinLED Dig2go](https://quinled.info/quinled-dig2go/) | Designed to be the quickest and easiest 5v addressable LEDs controller available! Powered simply by using a USB-C input (just like your phone!) for a true plug and play experience. Recommended for small projects up to 15W and very complete with built-in "power cut" circuit when the LEDs are off to minimize idle power consumption, LED data level-shifter, built in protection circuits (including fuses), IR receiver, high quality digital microphone with audio reactive effects and even has some easy to use expansion ports for extra buttons or for instance an I2C screen! All of this is housed in a high-quality custom plastic case (not 3D printed) and small enough to fit in the palm of your hand! Comes ready to go, pre-flashed with WLED and even combined with power supply and/or LED strip in different bundles! [Buy here!](https://dig2go.info/dig2go-buying-page/)
[QuinLED Dig-Uno](https://quinled.info/quinled-dig-uno/) | **2021 updated version!** DIY/Pre-Assembled board for digital LED driving. Integrated level shifters, temperature sensor option, Auto 5v-24v compatibility, pull-up/down GPIO and safety features such as a onboard fuse. Recommended to use (and comes with) with [custom QuinLED-ESP32](https://quinled.info/quinled-esp32/). Pre-assembled and pre-flashed with WLED [available to buy!](https://quinled.info/pre-assembled-quinled-dig-uno/). Aircoookie's personal recommendation for medium-size WLED projects.
[QuinLED Dig-Quad](https://quinled.info/quinled-dig-quad/) | **2021 updated version!** DIY/Pre-Assembled board for 4 (5) channel digital LED driving. Integrated level shifters, temperature sensor option, Auto 5v-24v compatibility, pull-up/down GPIO and power distribution terminals with 5x onboard fuses for easy LED power injection. Recommended to use (and comes with) with [custom QuinLED-ESP32](https://quinled.info/quinled-esp32/). Pre-assembled and pre-flashed with WLED [available to buy!](https://quinled.info/pre-assembled-quinled-dig-quad/). Aircoookie's personal recommendation for large-size WLED projects with advanced power and output requirements.
[QuinLED Dig-Octa](https://quinled.info/quinled-dig-octa/) | The Dig-Octa system is for your medium to very large projects! It comes fully pre-assembled and is the ideal board to drive 5v-24v digitally addressable LEDs. The system is composed of brain- and power-boards and is designed to be fully stackable in various configurations of both types of boards, to perfectly adapt to your needs. Some features are: 8 LED data-channels, built-in level-shifters and resistor switchers, Ethernet and external antenna WiFi, auto 5v-24v compatibility, high current handling (up to 50A to 100A!), fully fused inputs and outputs, dedicated relay circuit, I2C temperature sensor, and much more! Comes pre-flashed with WLED and is highly recommended for medium to very large projects. [Buy here!](https://quinled.info/quinled-dig-octa-available-here/)
[Simple WLED Board](https://github.com/wladwnt/wled) | Very simple DIY board, minimum of required components, option for 5V/12V LEDs. Easy to solder (no SMT components). Simple to understand connection schematics and pictures. Can be used with ESP8266 or ESP32 in D1 mini Format.
[sjm autoprod rgbw, rgbw2+, rgbw4](https://sjmautoprod.com/RGB-Controllers/rgbwX-Wi-Fi-Controllers.html) | Complete, fully-sealed, analog and digital controllers for vehicular use. rgbw has one RGBW channel, rgbw2+ has two analog, RGBW channels plus two/four addressable outputs (requires external 5V source for 5V LEDs). rgbw4 has four analog RGBW channels. 2+ and 4 support 12V or PWM/analog inputs and have internal PTC "fuses".
[WiFi Controlled Desk Lamp](https://github.com/stanoba/wifi-desk-lamp) | Open source PCB for WLED
[Yet Another WLED Controller](https://github.com/lizardsystems/yawl-controller) | Small and simple device for 5V addressable LED strips with minimum components and fully assembled by PCB manufacturing service in standard case. [Firmware is here](https://github.com/lizardsystems/yawl-controller/tree/main/firmware/WLED)

## Controllers on Tindie
🌜

| Name | Description ||
|---|---|---|
[WLED ESP32 universal controller](https://github.com/srg74/WLED-ESP32-universal-controller) | ready to buy on [Tindie](https://www.tindie.com/products/27056/), 100% compatible with WLED project. Integrated level shifter, 2 outputs for LEDs strips, 1 fused out for LED strip, relay for energy-saving, temperature sensor, PWM fan header, USB port for re-programing. Headers for shields to extend functionality. Available [shields for controller is here](https://www.tindie.com/stores/serg74/),  [Firmware is here](https://github.com/srg74/WLED-ESP32-universal-controller/tree/main/Firmware).
[ESP-01 WLED shield](https://www.tindie.com/products/24901/) | shield board for ESP-01 board, ready to buy on [Tindie](https://www.tindie.com/products/24901/). Integrated level shifter, 3 outputs for various configurations, mosfet for 1 analog channel, [Firmware is here](https://github.com/srg74/WLED-wemos-shield/tree/master/resources/Firmware/WLED_wemos_shield).
[WLED Wemos mini shield](https://github.com/srg74/WLED-wemos-shield/tree/master/resources/mini_shield) | shield board, ready to buy on [Tindie](https://www.tindie.com/products/22680/) also [Tindie EU](https://www.tindie.com/products/28777/). Integrated level shifter, 2 outputs for LEDs strips, 1 fused out for LED strip, resettable fuse for the development board, exposed I2C interface for display or sensors. Exposed pins Digital microphones. Works with Wemos D1 mini and D1-style ESP32 boards. [Firmware is here](https://github.com/srg74/WLED-wemos-shield/tree/master/resources/Firmware/WLED_wemos_shield). | <img width="240" alt="image" src="https://user-images.githubusercontent.com/91013628/213931748-bdec481c-c44e-48ea-84b0-aa733ad4e955.png">
[WLED Wemos shield](https://github.com/srg74/WLED-wemos-shield) | shield board, ready to buy on [Tindie](https://www.tindie.com/products/22307/) also [Tindie EU](https://www.tindie.com/products/28787/) or DIY 100% compatible with WLED project and WLED [sound reactive fork](https://github.com/atuline/WLED). Integrated level shifter, 4 outputs for LEDs strips, 1 fused out for LED strip, resettable fuse for the development board, exposed I2C interface for display or sensors, relay for energy-saving and 1-wire temperature sensor. Exposed pins for Analog and Digital microphones. Works with Wemos D1 mini and D1-style ESP32 boards. [Firmware is here](https://github.com/srg74/WLED-wemos-shield/tree/master/resources/Firmware/WLED_wemos_shield). | <img width="240" alt="image" src="https://user-images.githubusercontent.com/91013628/213931808-c8d6be07-ccb9-4acc-a5fa-3cdc37459591.png">
[WLED waterproof controller with external antenna](https://github.com/srg74/Controller-for-WLED-firmware) | DIY board, designed for use outside permanently and for longer range Wi-Fi connection. No SMD components means it is easier to solder for DIYers. 100% compatible with WLED project. Level shifter, fuse for LED strip, resettable fuse for Wi-Fi module, exposed I2C interface for display or sensors, relay for energy-saving and 1-wire temperature sensor. Build around ESP-07S module. [Firmware is here](https://github.com/srg74/WLED-wemos-shield/tree/master/resources/Firmware/WLED_wemos_shield)

## Controllers WLED can be installed to

!!! warning
    If the controller does not have a USB port and no firmware supporting wireless updates pre-installed, installing WLED to it requires an FTDI flasher and in some cases, soldering.

| Name | Chip | Description |
|---|---|---|
[ESPixelStick v3](https://forkineye.com/espixelstick-v3/) | ESP8266 | The ESPixelStick V3 is a WiFi Pixel and DMX single output controller built around the ESP8266 platform. It utilizes industry standard E1.31 sACN and DDP protocols for control of up to 680 WS2811 pixels (4 Universes) or 63 GECE Pixels.  The output passes through a built-in RS485 transceiver, allowing for driving DMX and differential Renard inputs (or using a differential receiver for long-distance between board and first pixel). The on board switching regulator allows you to power the ESPixelStick with 5V-24V -- Just match the voltage of the pixels you are using, no voltage configuration is required.  Note: Does _**not**_ come preconfigured with WLED, you must flash the ESP8266 yourself.
[SP108e v2](https://www.amazon.de/dp/B07KW1W68R) | ESP8285 | Hardware-Modification required and different versions exists! 8285-based 2M Controller that supports addressable RGBWW LED strips, also with CLK line (like ATA102). 5-24v DC input, 85mm x 45mm x 23mm. Vendors list spledapps 'Led Shop' as the supporting mobile application. Board is silk screened with 'SP108e'. No pads are exposed and a second processor is used to control the LEDs. Pin7 of that processor needs to be grounded to hold it in reset state. Then you can connect GPIO0 to GND and TX, RX, VCC, GND for flashing. Connect GPIO2 to R4 for DATA out and GPIO13 to R3 for CLK out. Flashed via PlatformIO, esptool. OTA updates work. Pics of pinout here: <https://github.com/psxde/sp108e-led-controller/raw/main/sp108ev2_inside.png>
SP501e | ESP8285 | 8285-based 1M Controller that supports both Addressable and PWM-based RGBWW LED strips. _Note that recent versions have 2M._ 5-24v DC input, 55mm x 26mm, sold under BTF lighting, RGBZone, etc. Vendors all list 'Fairynest' as the supporting mobile application. Board is silk screened with 'SP5XXe' but no other markings. Serial pads are exposed on the back-side of the board with GND and GPIO0 right next to each other and thus Flash access fairly straight forward. GPIO 0 must be pulled to GND at boot and throughout the flashing process.  I/O configuration: LEDPIN is 'GPIO3' for addressable (note this pin is limited to approx. 250 LEDs), BTNPIN is GPIO 1. PWM pin out for RGBWW: CW: 14, WW: 12, B: 13, R: 15 and G: 4. Flashed via PlatformIO, ESPHome and Tasmotizer. Pics of board here: <https://github.com/Operation760/SP501e-RGB-LED-Controller-/blob/master/SP501e_top_bottom_traced.jpg>  Flashing Connections: <https://github.com/tonyn0/sp501e-flashing/blob/main/sp501e%20flash.png>
[SP511e](https://www.aliexpress.com/item/32820185063.html) | ESP8285 | An ESP8285 2MB controller with 3 case buttons, built in mic, IR receiver, 38 key remote, and dual outputs. The dual outputs are connected to the same data pin. There is a step-by-step guide for [Installing WLED on SP511E Controller](https://github.com/scottrbailey/WLED-Utils/blob/gh-pages/sp511e_wled.md).
[ESP LED Strip WIFI Control Board [ESP Version]](https://www.electrodragon.com/product/esp-led-strip-board) | ESP8266 | Controller for addressable or analog LEDs (RGBW), 6-27VDC input, no level shifter, reset and boot buttons, enclosure. NOTE: Although this uses high-current transistors, they used jumpers on two of the connections so you are limited to their current rating (3A?).

## Other products WLED can be installed to

| Name | Chip | Description |
|---|---|---|
[Merkury MI-BW210-999W](https://www.walmart.com/ip/Merkury-Innovations-A21-Smart-Light-Bulb-75W-Color-LED-2-Pack/669037420) | ESP8285 | Tuya Style WiFi Led light bulb, Warm White + RGB. There are two versions of this same bulb sold in the same packaging only way to check is to look at the bulb, EBEQPW92 uses PWM led control and is compatible with WLED however EBEQPW06 uses an SM16716 chip and is not currently compatible with WLED. Managed to flash using tuya-convert and a custom WLED build with the following analog pinout: B:4, G:5, R:13, W:14. Extras disabled to allow OTA, OTA only way to flash this, programming headers are not internally available.
[Shelly RGBW2](https://shelly.cloud/wifi-smart-shelly-rgbw-2/) | ESP8266 | For "analog" LED use only! Runs on 12-24VDC. One button and one input. Pins: R=12, G=15, B=14, W=4. _Finished, commercial product that can be flashed._ [More info and flashing docs](https://tasmota.github.io/docs/devices/Shelly-RGBW2/#serial-connection)
[Athom 15W bulb](https://www.athom.tech/blank-1/15w-color-bulb) | ESP8266 (2M flash) | 15W bulb with RGB, warm white, and cold white LEDs. Compatible with all voltages, available form factors E27, B22 and [GU10](https://www.aliexpress.com/item/1005003512212258.html)

## Raw ESP8266/ESP32 boards

!!! tip
    While these can work like the controllers above without extra hardware, you might get flickering without adding an external levelshifter. Using them without a controller board/shield is only recommended if you like tinkering with electronic projects.

| Name | Chip | Description |
|---|---|---|
[Adafruit Feather Huzzah](https://learn.adafruit.com/adafruit-feather-huzzah-esp8266) | ESP8266 | General-purpose ESP8266 Board with USB, battery connector, etc.
[D1 mini-style ESP32](https://acrobotic.com/products/acr-00024) | ESP32 | A nice compact ESP32 development board. D1 mini compatible layout.
[ESP32 DevKitC v4](https://www.digikey.com/product-detail/en/espressif-systems/ESP32-DEVKITC-32D/1965-1000-ND/9356990) | ESP32 | The original ESP32 Development Board made by Espressif Systems.
[H803 WiFi](https://github.com/srg74/WLED/wiki/H803WiFi) | ESP8266 | ESP8266EX based controller with level shifter inside. Data pin GPIO1 Clock pin GPIO14. Tested with WS2813 strip and [Firmware fork is here](https://github.com/srg74/WLED/tree/H803WF).
NodeMCU-32s | ESP32 | The most common ESP32 development board. Works well, depending on the board you might have to press the "Boot" button while USB flashing
[Heltec WiFi Kit 8](https://heltec.org/project/wifi-kit-8/) | ESP8266 | Another alternative of ESP8266 board. OLED display 128X32 pixel, battery charger on board. Almost the same functionality and price as the Wemos board. Plus it can be used in projects with external batteries.
[NodeMCU](https://github.com/nodemcu/nodemcu-devkit-v1.0) | ESP8266 | Another popular ESP8266 development board. A bit bigger than the D1 and has pins pre-soldered. There are multiple versions with slight differences, not all are tested.
ESP-01 | ESP8266 | One of the first and cheapest ESP8266 boards available. **_Not recommended for general WLED installs_** (needs external USB/serial chip, voltage converter, only has 1mb of flash, so soon no wireless updates possible)
[Olimex ESP32 POE](https://www.olimex.com/Products/IoT/ESP32/ESP32-POE) | ESP32 | Ethernet (PoE) and WiFi, though usage of the ethernet port requires a custom compile. The PoE should not be used to power LEDs due to a maximum throughput of 4W. For most installations, standard ethernet should be used, supplying power through the 5V pin.
[QuinLED-ESP32](https://quinled.info/quinled-esp32/)| Custom design D1 Mini32 formfactor ESP32 module | Fed up with the bad quality of generic ESP32 modules on the market, designed my own "beefed up" version. Available in multiple versions: QuinLED-ESP32-AB (Antenna Board), QuinLED-ESP32-AE (Antenna External), QuinLED-ESP32-ABE (Antenna Board + Ethernet). Aircoookie's recommendation for running WLED.
[RE5V1C](https://www.itead.cc/sonoff-re5v1c.html) | ESP8285 | 5v DC input - onboard 10A relay
[TwilightLord-ESP32](https://www.tindie.com/products/22968/)| ESP32 | ESP32 Dev Board with latest WROOM-32E module, USB Type-C, 800mA LDO, 8MB flash and PTC fused. D1 Mini32 form factor and compatible pin out.[16MB Flash version also available](https://www.tindie.com/products/23037/)
[Wemos D1 mini](https://docs.wemos.cc/en/latest/d1/d1_mini.html) | ESP8266 | An affordable ESP8266 development board. Aircoookie's recommendation for running WLED if you want an ESP8266 board. Current version: 3.1.0
[Wemos D1 mini Pro](https://docs.wemos.cc/en/latest/d1/d1_mini_pro.html) | ESP8266 | A newer development board with an external antenna connector. Works very well with WLED. Recommended if your signal strength is too low with another board. Current version: 2.0.0. Version 1.0.0 has the same form factor as the D1 mini.
[WT32-ETH01](https://www.aliexpress.com/wholesale?&SearchText=wt32-eth01) | ESP32 | **Under development!** Ethernet (non-PoE) and WiFi enabled alternative to the Olimex boards, for 1/4 the cost. Features no PoE, and requires initial flashing of a custom compiled image using a FTDI or similar USB to serial converter.

## ESP32 boards on Tindie
🌜

| Name | Description ||
|---|---|---|
[ESP32 mini dev board 16mb](https://github.com/srg74/ESP32-mini-SerKo) | by SerKo (aka Serg). Buy on [Tindie US](https://www.tindie.com/products/28858/) or [Tindie EU](https://www.tindie.com/products/28788/). ESP32 Dev Board with latest WROOM-32E module, USB Type-C, PTC fused, over-voltage protection. D1 Mini32 form factor and compatible [pin out](https://github.com/srg74/ESP32-mini-SerKo/blob/main/Resources/ESP32_mini_board_pinout.pdf) | <img width="240" alt="image" src="https://user-images.githubusercontent.com/91013628/213931205-520ed9e9-9195-4738-9a05-839ad7d57791.png">
[ESP32 pico board with digital microphone](https://github.com/srg74/WLED-ESP32-pico) | by SerKo (aka Serg). Buy on [Tindie US](https://www.tindie.com/products/serg74/esp32-wled-pico-board/) or [Tindie EU](https://www.tindie.com/products/29131/). ESP32-pico-D4 development board with integrated ics-43434 microphone | <img width="240" alt="image" src="https://user-images.githubusercontent.com/91013628/213931625-0804dc5d-6bce-4c37-ab00-52e11573a2b6.png">

## Microphones on Tindie
🌜

| Name | Description ||
|---|---|---|
Digital I2S microphone ICS-43434 | by SerKo (aka Serg). Buy on [Tindie US](https://www.tindie.com/products/serg74/digital-i2s-microphone-ics-43434-add-on/) or [Tindie EU](https://www.tindie.com/products/28781/). | <img width="240" alt="image" src="https://user-images.githubusercontent.com/91013628/213933631-2e613a69-9f30-40c8-a297-13563843b56f.png"> 
Digital I2S PDM microphone SPM1423 | by SerKo (aka Serg). Buy on [Tindie EU](https://www.tindie.com/products/28781/). | <img width="240" alt="image" src="https://user-images.githubusercontent.com/91013628/213933684-f6c83270-4621-435c-9ddc-0fe5807b54a2.png"> 

## Useful boards and addons

| Name | Description |
|---|---|
[ESP32 Ethernet Network Shield](https://www.tindie.com/products/30385/)| Ethernet Shield (10/100Mbps) for ESP32 boards. Stackable with D1 Mini32 form factor boards.
[Logic Level Shifter Board](https://www.tindie.com/products/sjmelectronics/logic-level-converter-level-shifter) | A simple level shifter board. Updated version has selectable data-pin resistors.
[Logic Level Shifter Shield](https://www.tindie.com/products/sjmelectronics/logic-level-converter-shield)| Logic level shifter shield for Seeed Studio ESP32-C3 and D1 Mini format dev boards. Updated version has selectable data-pin resistors.
[WIZmote remote control](https://www.google.com/search?q=wizmote) | Remote control using radio network. Compatible with WLED (vesions 0.14.0-beta3 and above). No additional receiver required.

## Compatible PC RGB Fans and ARGB accessories

| Brand | Model | Comments |
|---|---|---|
Corsair | HD120 Fan | Uses WS2812B, data-in only
PCCOOLER | Moonlight 5-pack Fans | Uses WS2812B, includes Data-out connector to keep each fan uniquely addressable if wired in series like traditional LED strips
Any | 5v 3-pin ARGB for PC | Any PC RGB device that supports the 5v 3-pin ARGB motherboard header should work fine with WLED. All the major motherboard vendors support the Corsair HD120 and PCCOOLER fans listed, so we can safely assume any device that supports motherboard ARGB 5V 3-Pin standard will work with WLED.

## Levelshifters

| Name | Description |
|---|---|
SN74AHCT125 | Aircoookie's recommended levelshifter. Often used in DIY and commercial controllers. [sjm Level Shifter Board](https://www.tindie.com/products/sjmelectronics/logic-level-converter-level-shifter)
SN74AHCT32 | Same pinout as above can be used. This is just an OR gate, but any AHCT gate can be used if inputs are connected appropriately. ;)
SN74HCT125N | Slower, cheaper version. Works just as well for WS2812, but not recommended for APA102.
SN74LVC2T45 | Modern bus transceiver with voltage translation [Yet Another WLED Controller](https://github.com/lizardsystems/yawl-controller)
Amplifier/Splitter | These have been tested and do work. [More info here.](https://discord.com/channels/473448917040758787/719873873071308821/1278797679656439849) - [Example product](https://www.amazon.com/BTF-LIGHTING-WS2812B-Amplifier-Support-addressable/dp/B0B5ZSSFR7)
TXS0102, TXS0108 | Not recommended: these bidirectional levelshifters do work but only for short data lines (less than 50cm).
[F-Amp](https://pixelcontroller.com/store/accessories/54-famp-xconnect.html) | Level shifter/data booster

!!! warning
    I2C shifters are generally too slow for addressable LEDs, so don't use them.  
    ![No_I2C_Shifter](../assets/images/content/NoI2Cshifter.jpg)  
    If you must: there is a [hack to make them work on short data lines](https://wled.discourse.group/t/levelshifter-analysis/11871/12)

Further reading:
[Logic Level Shifters for Driving LED Strips](https://electricfiredesign.com/2021/03/12/logic-level-shifters-for-driving-led-strips/)

How to connect Levelshifters:
![LS_32_R2](../assets/images/content/LS_32_R2.jpg)
![74AHCT125 one output](../assets/images/content/pic1.jpg)
![74AHCT125 two outputs](../assets/images/content/pic2.jpg)
![TXS0108](../assets/images/content/pic3.jpg)
![LS_245_R2](../assets/images/content/LS_245_R2.jpg)

## USB/TTL adapters


| Name | Description |
|---|---|
[CH340](https://www.aliexpress.com/item/32761423124.html) | CH340 module instead of CP2102, PL2303 or FTDI/FTDT. The CH340 can deliver more current which is needed while the flash process depending on the board type. The timing is also much more stable. **For boards with an USB/TTL adapter onboard this is NOT needed**
[ESP uploader](https://github.com/srg74/ESP-uploader) |  CP2102N module. Same USB to UART converter as many recent Dev boards using. Featuring latest USB-C connector. For use with many ESP32, ESP8266, ESP8255 and Tuya based modules. 3.3V logic and 5V power pass through for custom boards.

## Miscellaneous

Sorting: Sensors, Displays, Actuators

| Name | Description |
|---|---|
[HC-SR501](https://www.aliexpress.com/wholesale?catId=0&SearchText=HC-SR501) | PIR sensor with adjustable sensitivity and on time delay (suitable as a button).
[HC-SR602](https://www.aliexpress.com/wholesale?catId=0&SearchText=HC-SR602) | PIR sensor (not suitable as a button but can be used with _PIR sensor_ usermod).
[TSOP38238](https://www.aliexpress.com/item/32834341300.html) | IR receiver compatible with most IR remotes.
[SSD1305](https://www.aliexpress.com/wholesale?catId=0&SearchText=SSD1305) | I2C display, can be used with [_4 Line Display_ usermod](https://github.com/Aircoookie/WLED/tree/master/usermods/usermod_v2_four_line_display).
[SSD1306](https://www.aliexpress.com/wholesale?catId=0&SearchText=SSD1306) | I2C & SPI display, can be used with _4 Line Display_ usermod.
DS18B20 | Recommended temperature sensor for use with WLED. Compatible with the [Temperature usermod](https://github.com/Aircoookie/WLED/tree/master/usermods/Temperature)
[Display shield](https://www.tindie.com/products/27112/) | Various configurations. Compatible with the [ESP32 WLED dev board](https://www.tindie.com/products/27056/) also can be used with ESP32 mini dev boards.
[12V Relay & Fuse board](https://shop.myhome-control.de/Relais-Board-fuer-WLED-Controller-12V/HW10011)|Integrates two relays and two 10 A fuses. Suitable for WLED setups with 12 V LED Strips.
[5V relay](https://www.aliexpress.com/wholesale?catId=0&SearchText=5v+relay+module) | Relay module. Some will require 5V to trigger so you will need level-shifted output (similar as for LEDs) for proper functionality or a circuit with transistor or MOSFET.
[5V Relay & Fuse board](https://shop.myhome-control.de/Relais-Board-fuer-WLED-Controller-5V/HW10005)|Integrates two relays and two 10 A fuses. Suitable for WLED setups with 5V LED Strips.
