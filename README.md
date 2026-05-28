# PRM Client Firmware Installer

Client-facing firmware installer for the Pocket Railway Museum Wemos D1 mini locomotive controller.

## Client flow

1. Install USB driver.
2. Connect the Wemos D1 mini locomotive controller.
3. Install firmware from the browser.
4. Connect to the default locomotive Wi-Fi network:

   PRM LOCOMOTIVE

5. Open:

   http://192.168.4.1

6. Rename the locomotive Wi-Fi and optionally set a password.
7. Reconnect to the new Wi-Fi name and open the PRM controller app.

## Firmware file

Replace this file with your compiled Arduino binary:

firmware/wemos-d1-mini-firmware.bin

## Hosting

This is a static site. It can be hosted on GitHub Pages, Netlify, Vercel, or embedded later in the PRM website.

Keep these paths together:

- index.html
- styles.css
- manifest.json
- firmware/wemos-d1-mini-firmware.bin
