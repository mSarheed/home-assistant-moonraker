# Moonraker integration with Home Assistant

Little project to connect my 3D printer running Klipper + Moonraker to Home Assistant. Heavily inspired by **@denkyem**'s [Home Assistant Moonraker](https://github.com/denkyem/home-assistant-moonraker).

![Screenshot](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/lovelace_dashboard_screenshot.png?raw=true)

## Setup

- HACS (for installing custom component)
- Synthwave Hass theme
- **@thosmasloven**'s [Lovelace Card Mod](https://github.com/thomasloven/lovelace-card-mod)
- **@kalkih**'s [Mini Graph Card](https://github.com/kalkih/mini-graph-card)
- **Sonoff S26** with **ESPHome** for powering the 3D printer on/off

## Lovelace cards

> **Horizontal Stack Card**

For buttons to stop, FW reset, pause, resume and cancel. [Card code](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/horizontal-stack-lovelace.yaml)

> **Picture Entity Card (live stream webcam)**

For livestream feed of webcam connected to MCU. [Card code](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/picture-entity-webcam.yaml)

> **Picture Entity Card (STL thumbnail)**

Showing thumbnail of currently printing STL. Make sure slicer is configured for this. [Card code](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/picture-entity-thumbnail.yaml)

> **Glance Card (info and Sonoff Power Plug)**

Showing info and button to turn on and off the Sonoff S26 Power Plug. [Card code](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/glance-card.yaml)

> **Gauge Card (printing progress)**

Showing currently % of printing progress. Changes color depending on % of progress [Code card](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/gauge-card.yaml)

> **Temperature Graph (hotend and bed)**

Using mini-graph-card component, to show graph of hotend and bed temp. [Code card](https://github.com/thehiddentruth/home-assistant-moonraker/blob/main/mini-graph-card.yaml)
