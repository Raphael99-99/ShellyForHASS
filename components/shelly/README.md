![stability-wip](https://img.shields.io/badge/stability-work_in_progress-lightgrey.svg?style=for-the-badge)

# Shelly smart home platform for HASS
This platform add components for Shelly smart home devices to Home Assistant.

## Features
- Discover devices
- Monitor status (state, temperature, humidity, power etc.)
- Control (turn on/off, dim, color, etc)

## Devices supported
- Shelly 1
- Shelly 2 (relay or roller mode)
- Shelly 4
- Shelly PLUG
- Shelly BULB
- Shelly RGBWW
- Shelly RGBW2
- Shelly H&T
- Shelly 2LED (not tested)
- Shelly 2.5 (not tested)
- Shelly PLUG S (not tested)

## Installation

### (not working yet) Install with Custom Updater
Do you you have [Custom updater](https://github.com/custom-components/custom_updater) installed? Then you can use the service [custom_updater.install](https://github.com/custom-components/custom_updater/wiki/Services#install-element-cardcomponentpython_script) with the parameter {"element":"shelly"} to install Shelly.

### Install manualy
1. Install this platform by creating a `custom_components` folder in the same folder as your configuration.yaml, if it doesn't already exist.
2. Create another folder `shelly` in the `custom_components` folder. Copy all 5 Python (.py) files into the `shelly` folder. Use `raw version` if you copy and paste the files from the browser.

## Configure
When you have installed shelly and make sure it exist under `custom_components` folder it is time to configure it in Home Assistant.

It is very easy, just add this to `config.yaml`
```
shelly:
```
(Options will be added later)

## Restart Home Assistant
Now yot should restar Home Assistant to load shelly

Shelly will discover all devices on your LAN and show them as light, switch and cover in Home Assistant.

## Feedback
Please give us feedback on info@styrahem.se or Facebook groups: [Shelly group (Swedish)](https://www.facebook.com/groups/ShellySweden) or [Shelly support group (English)](https://www.facebook.com/groups/ShellyIoTCommunitySupport/)