---
title: Welcome to WLED MoonModules & Sound Reactive
hide:
  - navigation
  - toc
---

<p align="center">
  <img src="assets/images/ui/headers/wled_logo_akemi.png">
  <a href="https://github.com/MoonModules/WLED/releases"><img src="https://img.shields.io/github/release/MoonModules/WLED.svg?style=flat-square"></a>
  <a href="https://raw.githubusercontent.com/MoonModules/WLED/mdev/LICENSE"><img src="https://img.shields.io/github/license/MoonModules/wled?color=blue&style=flat-square"></a>
  <a href="https://wled.discourse.group"><img src="https://img.shields.io/discourse/topics?colorB=blue&label=forum&server=https%3A%2F%2Fwled.discourse.group%2F&style=flat-square"></a>
  <a href="https://discord.gg/4CQRmfR"><img src="https://img.shields.io/discord/700041398778331156.svg?colorB=blue&label=discord&style=flat-square"></a>
  <a href="https://github.com/MoonModules/WLED"><img src="https://img.shields.io/badge/source-github-blue.svg?style=flat-square"></a>
  <a href="https://github.com/Aircoookie/WLED-App"><img src="https://img.shields.io/badge/app-wled-blue.svg?style=flat-square"></a>
  <a href="https://gitpod.io/#https://github.com/MoonModules/WLED"><img src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?style=flat-square&logo=gitpod"></a>
</p>
  
# Welcome to WLED MoonModules

MoonModules/WLED is a fork from Aircoookie/WLED which contains latest merge of v0.14 of WLED with additional features.

This fork is created by members of the Atuline/WLED team to make development against v0.14 possible while still preserving Atuline/WLED v0.13 as a stable and supported version. The Atuline/WLED fork is also called WLED SR (Sound Reactive).

More info [here](/moonmodules/what-is-moonmodules/).

## Good to know
* Aircoookie/WLED will be referred to as WLED AC or upstream in this documentation
* MoonModules/WLED will be referred to as WLED MM in this documentation
* Atuline/WLED will be referred to as WLED SR in this documentation (As this was called WLED Sound Reactive)
* This documentation is a fork of WLED AC documentation ([kno.wled.ge](http://kno.wled.ge))
* The menu options Welcome, Basics, Features, Interfaces, Advanced and About originate from upstream
* The menu options Usermods, MoonModules, 2D, Sound Reactive and WLEDSR are added
* Usermods are the readme.md files of usermods and will move to upstream (see https://github.com/Aircoookie/WLED/pull/2965)
* WLEDSR is a 1:1 copy of [WLED SR Wiki](https://github.com/atuline/WLED/wiki) and will slowly moved to menu items more to the left (updated to 0.14 functionality)
* MoonModules, 2D and SoundReactive might also be moved to the left, depending on how upstream will organise these topics
* To see where this documantation differs from upstream documentation the following icons will be used in Welcome, Basics, Features, Interfaces, Advanced and About:🌜: Specific to WLED MM, 🎸: Specific to WLED SR
* Hint: search on 🌜or 🎸 to find WLED MM or AC specific info

Disclaimer: using this software is the users responsibility as it is not bug free. Therefore contributors of this repo are not reliable for anything including but not limited to spontaneous combustion of the entire led strip, the house and the inevitable heat death of the universe

Join the Discord server to discuss everything about WLED MM and SR!

<a href="https://discord.gg/HgAsbvWuJ3"><img src="https://discordapp.com/api/guilds/700041398778331156/widget.png?style=banner2" width="25%"></a>

WLED Aircoookie welcome 👇

# Welcome to my project WLED! ✨

A fast and feature-rich implementation of an ESP8266/ESP32 webserver to control NeoPixel (WS2812B, WS2811, SK6812) LEDs or also SPI based chipsets like the WS2801 and APA102!

## ⚙️ Features

- WS2812FX library integrated for over 100 special effects  
- FastLED noise effects and 50 palettes  
- Modern UI with color, effect and segment controls  
- Segments to set different effects and colors to parts of the LEDs  
- Settings page - configuration over network  
- Access Point and station mode - automatic failsafe AP  
- Up to 3 LED outputs per ESP8266 instance and 10 LED outputs per ESP32 instance
- Support for RGBW strips  
- Up to 250 user presets to save and load colors/effects easily, supports cycling through them.  
- Presets can be used to automatically execute API calls  
- Nightlight function (gradually dims down)  
- Full OTA software updatability (HTTP + ArduinoOTA), password protectable  
- Configurable analog clock + support for the Cronixie kit by Diamex  
- Configurable Auto Brightness limit for safer operation  
- Filesystem-based config for easier backup of presets and settings
- Native [Home-Assistant integration](https://www.home-assistant.io/integrations/wled/): [![Start native Homeassistant integration configuration](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start?domain=wled)

## 💡 Supported light control interfaces

- [WLED app](https://github.com/Aircoookie/WLED-App) for [Android](https://play.google.com/store/apps/details?id=com.aircoookie.WLED) and [iOS](https://apps.apple.com/us/app/wled/id1475695033)
  - Alternatively, WLED Native app made by community member [Moustachauve](https://github.com/Moustachauve)
    - For [Android](https://play.google.com/store/apps/details?id=ca.cgagnier.wlednativeandroid) [[Source]((https://github.com/Moustachauve/WLED-Native-Android))]
    - For [iOS](https://apps.apple.com/us/app/wled-native/id6446207239) [[Source]((https://github.com/Moustachauve/WLED-Native-iOS/))]
- [JSON](/interfaces/json-api) and [HTTP request](/interfaces/http-api) APIs  
- [MQTT](/interfaces/mqtt)  
- [Blynk IoT](/interfaces/blynk)  
- [E1.31](/interfaces/e1.31-dmx), [Art-Net](/interfaces/e1.31-dmx), DDP and [TPM2.net](/interfaces/udp-realtime)
- [Hyperion](https://github.com/hyperion-project/hyperion.ng)
- [UDP realtime](/interfaces/udp-realtime)
- [Alexa voice control (including dimming and color)](/advanced/remote-access-ifttt)
- [Sync to Philips Hue lights](/interfaces/philips-hue)
- Adalight (PC ambilight via serial) and TPM2  
- [Sync color of multiple WLED devices (UDP notifier)](/interfaces/udp-notifier)
- [Infrared remotes (24-key RGB, receiver required)](/interfaces/infrared)
- Simple timers/schedules (time from NTP, timezones/DST supported)  

## 📲 Quick start guide and documentation

See the [getting started](/basics/getting-started) page!

[On this page](/basics/tutorials) you can find excellent tutorials made by the community and helpful tools to help you get your new lamp up and running!

## 🖼️ User interface

<img src="assets/images/ui/headers/macbook-pro-space-gray-on-the-wooden-table.jpg" width="50%"><img src="assets/images/ui/headers/walking-with-iphone-x.jpg" width="50%">

## 💾 Compatible hardware

See [here](/basics/compatible-hardware)!

## ✌️ Other

Licensed under the MIT license  
Credits [here](/about/contributors)!

Join the Discord server to discuss everything about WLED!

<a href="https://discord.gg/QAh7wJHrRM"><img src="https://discordapp.com/api/guilds/473448917040758787/widget.png?style=banner2" width="25%"></a>

Check out the WLED [Discourse forum](https://wled.discourse.group)!  
If WLED MM really brightens up your every day, you can [![Paypalbadge](https://img.shields.io/badge/send%20me%20a%20small%20gift-paypal-blue.svg?style=flat-square)](https://paypal.me/moonmodules)

!!! danger "Disclaimer"
    If you are sensitive to photosensitive epilepsy it is not recommended that you use this software.  
    In case you still want to try, don't use strobe, lighting or noise modes or high effect speed settings.  
    As per the MIT license, I assume no liability for any damage to you or any other person or equipment.  
