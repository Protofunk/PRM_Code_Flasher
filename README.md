# PRM Code Flasher - PRM Page Style

This is the standalone top-level firmware flasher page intended to be opened from the Wix code page in a new tab.

It includes:
- PRM-style intro section
- experimental feature note
- hardware recommendation block
- link to the electronics guide
- firmware installer using ESP Web Tools
- post-flash Wi-Fi setup instructions

## Electronics link

https://www.pocketrailwaymuseum.com/electronics

## Firmware file

Replace this file with your compiled Arduino binary:

firmware/wemos-d1-mini-firmware.bin

## Homepage link

A bottom button links back to https://www.pocketrailwaymuseum.com/

## Port selection hint

When the browser asks for a serial port, the Wemos D1 mini usually appears as something like `USB Serial (COM...)` on Windows. On Mac it may appear as `USB Serial` or `wchusbserial`.

## Fonts

This version imports Google Fonts:
- Suez One for titles
- Roboto Bold for main text

