# FilaPropus Waage WebFlash

Browser-based flashing for the FilaPropus Waage (ESP32) using ESP Web Tools.

## What this does

- Flashes firmware and LittleFS directly from the browser
- Works in Chrome or Edge via WebSerial

## Files

- `index.html` - WebFlash UI
- `manifest.json` - ESP Web Tools manifest
- `bin/` - Firmware and LittleFS .bin artifacts

## Usage

Open `index.html` in a web server (GitHub Pages, nginx, etc.), then click **Flash**.

GitHub Pages: https://janez76.github.io/waage-webflash/

## Build artifacts

This repo expects:

- `bin/upgrade_filapropus_firmware_v1.3.0.bin`
- `bin/upgrade_filapropus_website_v1.3.0.bin`

## Notes

- The manifest uses the ESP32 offsets `0x10000` (firmware) and `0x290000` (LittleFS).
- WebSerial requires HTTPS or `localhost`.
