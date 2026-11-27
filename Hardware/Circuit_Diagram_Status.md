# Circuit diagram status

**Pending:** A verified circuit diagram cannot be drawn accurately until the exact ESP32 board, PMS5003 connector/pinout, UART pin selection, OLED controller, I2C address, and SDA/SCL pins are confirmed.

The intended signal architecture is:
- PMS5003 ↔ ESP32: UART (exact TX/RX mapping pending).
- ESP32 ↔ 1.3-inch OLED: I2C (SDA/SCL mapping and address pending).
- ESP32: USB power confirmed.

Add a labelled diagram based on the actual assembled wiring before final submission.
