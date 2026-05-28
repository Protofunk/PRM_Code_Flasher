# Wemos D1 Mini Web Firmware Installer

This is a static website starter for flashing precompiled Arduino firmware to a Wemos D1 mini / ESP8266 from the browser.

## What clients need

- Chrome or Edge on desktop
- A data-capable USB cable
- CH340 driver if their Wemos clone is not detected

## What you need to do

1. Open your Arduino project.
2. Select the correct ESP8266 board, usually something like:
   - LOLIN(WEMOS) D1 R2 & mini
   - Flash size: commonly 4MB, depending on your board
3. Export the compiled binary from Arduino IDE.
4. Rename the exported `.bin` to:

   firmware/wemos-d1-mini-firmware.bin

5. Replace the placeholder file in this folder.
6. Host this whole folder on GitHub Pages, Netlify, Vercel, or your own HTTPS site.

## Important

The website does not compile Arduino code. It flashes your already-compiled `.bin` firmware.

That is better for client use because your libraries, board core, and project code are already baked into the firmware binary.

## Testing locally

Because browser serial features are stricter on permissions, test from an HTTPS site where possible.
GitHub Pages is a simple option.

## Recommended firmware setup flow

For client projects, avoid hardcoding Wi-Fi and server details.

Instead, make the flashed firmware start a setup access point after first boot, for example:

TrainController-Setup

Then expose a small configuration page at:

192.168.4.1

Store:
- Wi-Fi SSID
- Wi-Fi password
- WebSocket or HTTP server URL
- Device name
- Optional train ID

This way you can use one generic firmware for many clients.
