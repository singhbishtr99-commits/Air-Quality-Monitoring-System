# Installation and Setup Guide

This guide describes the intended workflow. Complete the pending hardware details before wiring or uploading firmware.

## Software
- Arduino IDE (version to be recorded).
- ESP32 board support package (version to be recorded).
- PMS5003 library or custom UART parser (selection pending).
- OLED display library compatible with the exact display controller (selection pending).

## Hardware setup checklist
- [ ] Identify the exact ESP32 development-board model.
- [ ] Check the PMS5003 datasheet and connector pinout.
- [ ] Confirm PMS5003 supply requirements and UART signal levels.
- [ ] Confirm ESP32 UART RX/TX pin mapping.
- [ ] Identify the OLED controller and confirm I2C address.
- [ ] Confirm OLED SDA/SCL pins for the selected ESP32 board.
- [ ] Verify common ground and all supply voltages before powering on.
- [ ] Add a labelled circuit diagram to `Hardware/`.

## Firmware workflow
1. Open `Source_Code/Air_Quality_Monitor.ino` in Arduino IDE.
2. Add the confirmed libraries.
3. Set the verified UART and I2C pin definitions.
4. Implement PMS5003 frame reception and validation.
5. Implement OLED initialization and display of PM1.0, PM2.5 and PM10.
6. Select the correct ESP32 board and USB/serial port.
7. Compile and upload.
8. Test in a safe, ventilated environment and record the test conditions and observations.

## Evidence to add
- Actual assembled-project photographs.
- A labelled wiring/circuit diagram.
- Firmware version and library versions.
- Dated observations and readings.
- Any limitations or issues found during testing.

## Caution
Do not assume example pin assignments are universal. Verify every connection against the exact module and board documentation. Avoid exposing ESP32 GPIO pins to signals above their permitted input voltage.
