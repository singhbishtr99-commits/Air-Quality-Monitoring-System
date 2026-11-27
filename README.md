# IoT-Based Air Quality Monitoring System Using ESP32 and PMS5003

A student project developed at **KR Mangalam University**.

## Team
- Piyush
- Rahul Singh Bisht
- Sanskriti Verma
- Kavya Pandey
- Anurudh
- Harshit Rana

## Project overview
This project is intended to measure particulate-matter concentrations using a Plantower PMS5003 sensor, process the received readings with an ESP32, and present PM1.0, PM2.5 and PM10 values on a 1.3-inch I2C OLED display.

## Confirmed hardware details
| Item | Confirmed detail |
|---|---|
| Microcontroller | ESP32 |
| Particulate sensor | Plantower PMS5003 |
| Display | 1.3-inch OLED, I2C |
| ESP32 power | USB |
| Displayed parameters | PM1.0, PM2.5, PM10 |

## Repository structure
- `Report/` — project report in PDF and editable DOCX formats.
- `Source_Code/` — Arduino sketch placeholder and code notes.
- `Hardware/` — component list and circuit/wiring status.
- `Images/Project_Photos/` — add actual project photographs here.
- `Documentation/` — working principle and setup checklist.

## Current status and pending information
This repository is a documentation starter pack. The following details must be confirmed from the actual build before final submission:
- Exact ESP32 board model and selected UART pins.
- PMS5003 power and signal wiring, including any level-shifting requirements.
- OLED controller/model, I2C address, and SDA/SCL pin mapping.
- Exact Arduino libraries and firmware implementation.
- Actual photographs and circuit diagram.
- Experimental readings, test conditions, and any calibration/validation data.
- Whether any AQI value is calculated. This project currently documents PM concentration readings only; it does not claim an AQI calculation.

## Safety and accuracy note
Do not connect modules based only on the example pin names in draft documentation. Verify the pinout and voltage requirements for the exact ESP32 board and PMS5003 module. Never connect a 5 V signal directly to an ESP32 GPIO unless the board/module documentation confirms it is safe.

## Getting started
1. Confirm the wiring for the exact modules.
2. Install the Arduino IDE and ESP32 board support.
3. Add the required libraries after identifying the chosen display and PMS5003 libraries.
4. Complete `Source_Code/Air_Quality_Monitor.ino`.
5. Upload the sketch to the ESP32 over USB.
6. Verify the three PM readings against the sensor documentation and record test observations.
7. Add genuine circuit images and project photographs.

See `Documentation/Installation_Guide.md` and `Hardware/Components_List.md`.
