# Components List

| Component | Purpose | Status / details |
|---|---|---|
| ESP32 development board | Main controller; receives sensor data and drives display | Confirmed; exact board variant pending |
| Plantower PMS5003 | Measures particulate matter and reports PM1.0, PM2.5 and PM10 | Confirmed; exact connector/pinout pending |
| 1.3-inch OLED display | Displays particulate readings | Confirmed; I2C interface |
| USB cable and USB power source | Powers ESP32 during operation/programming | Confirmed |
| Jumper wires | Electrical connections | To be confirmed |
| Breadboard / mounting base | Prototype assembly | To be confirmed |

## Pending technical specifications
- PMS5003 supply voltage and connector pinout: verify against the exact module datasheet.
- ESP32 UART pins: pending.
- OLED SDA/SCL pins and I2C address: pending.
- Additional components such as level shifters, resistors, or connectors: pending after wiring review.
