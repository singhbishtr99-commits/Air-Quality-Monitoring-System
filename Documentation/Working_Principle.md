# Working Principle

## 1. Particulate sensing
The PMS5003 is a particulate-matter sensor that uses a laser-scattering measurement method. Particles passing through its sensing chamber scatter light; the sensor processes the optical signal and reports particulate-matter concentration data.

## 2. Data communication
The intended design connects the PMS5003 to the ESP32 through a UART serial interface. The ESP32 receives the sensor's data frame and should validate the frame before using its values. Exact UART pins, baud rate, and frame implementation must be confirmed from the module documentation and final firmware.

## 3. Processing and display
The ESP32 extracts the PM1.0, PM2.5 and PM10 values and presents them on a 1.3-inch OLED using I2C communication. The OLED's I2C address and SDA/SCL pin mapping remain pending.

## 4. Power
The ESP32 is powered through USB. The power arrangement for the PMS5003 and OLED, including voltage compatibility and grounding, must be verified against the exact hardware documentation.

## Data flow
PMS5003 particulate sensing → UART data transfer → ESP32 data validation/processing → I2C communication → 1.3-inch OLED display.

## Important distinction
PM concentration readings are not automatically the same as an official Air Quality Index (AQI). The current project scope is to display PM1.0, PM2.5 and PM10. An AQI feature should only be added if a documented standard, averaging period, and calculation method are implemented.
