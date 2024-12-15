# Getting Started w/ my Smart home Configuration

## Services Utilized

- [ZWave JS](https://github.com/zwave-js)
- [Home Assistant](https://www.home-assistant.io)
- [Node-Red](https://nodered.org)
- [ESP Home](https://esphome.io)

## ZWave JS UI

ZWave integration for Home Assistant

## Home Assistant

Home Assistant is the workhorse of the smart home. It is where all of the integrations
into third party services / sensors live. This is where I configure any integrations
such as Philips Hue, SONOS, or the current wind speed.

## Node Red

Node Red is the automation work horse it has a great UI and an intuitive flow
that makes it super simple to get started drawing and laying out automations.
I also like the fact that I can test an automation super simply by adding the
timestamp start point and click and test out that things work.
I recommend this if the Home Assistant automations seem cumbersome or not intuitive.

## ESP Home

ESP Home is a system to control micro computers (ESP8266/ESP32 and RP2040) by
simple yet powerful configuration files. This will then allow you to control
these micro computers remotely through Home Automation systems. In my case Home-Assistant.
