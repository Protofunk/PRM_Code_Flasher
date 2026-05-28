# PRM Client Firmware Installer - Embed Ready

This version is designed to work well as a standalone GitHub Pages installer and later inside an iframe.

The visual style is intentionally quieter:
- light PRM-style base
- compact header
- no promotional hero block
- clear technical steps
- reduced marketing language

## Client flow

1. Install USB driver.
2. Connect the Wemos D1 mini locomotive controller.
3. Install firmware from the browser.
4. Connect to the default locomotive Wi-Fi network:

   PRM LOCOMOTIVE

5. Optional: open http://192.168.4.1 and rename the locomotive Wi-Fi or set a password.
6. Reconnect to the locomotive Wi-Fi and open the PRM controller app.

## Forgotten password

Connect the Wemos D1 mini to USB and repeat the install steps. When prompted, choose the clean install / erase option. The controller returns to the default Wi-Fi network: PRM LOCOMOTIVE.

## Firmware file

Replace this file with your compiled Arduino binary:

firmware/wemos-d1-mini-firmware.bin
