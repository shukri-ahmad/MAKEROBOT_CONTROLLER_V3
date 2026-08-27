# MAKEROBOT Controller — Bluetooth + Data Reader

This upgraded version combines:
- Robot control over micro:bit Bluetooth UART
- Incoming string-data display from the micro:bit
- Latest-value display
- Scrolling received-data log
- CSV export
- A/B and directional controls
- Automatic `S` stop command when a control button is released
- Keyboard controls

## Bluetooth UUIDs

Nordic UART Service:
- Service: 6e400001-b5a3-f393-e0a9-e50e24dcca9e
- TX (browser -> micro:bit): 6e400002-b5a3-f393-e0a9-e50e24dcca9e
- RX (micro:bit -> browser): 6e400003-b5a3-f393-e0a9-e50e24dcca9e

## Control commands

F = Forward
B = Backward
L = Left
R = Right
S = Stop
A = A button
B = B button

Commands are sent with a newline.

## Receiving data

The micro:bit can send strings such as:

Temperature: 28
Distance: 35
Speed: 80

Each newline-delimited string appears in the Received String Data panel.

## Deploy to GitHub Pages

Replace the existing `index.html` in the MAKEROBOT_CONTROLLER repository with this file, then enable GitHub Pages for the repository.

Web Bluetooth requires HTTPS (GitHub Pages satisfies this). Chrome/Edge are recommended.
