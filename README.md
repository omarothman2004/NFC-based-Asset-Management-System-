# NFC Workshop Asset & Tool Tracker

A professional-grade, custom-designed 13.56MHz NFC reader and inventory tracking terminal built from scratch. This project bridges hardware RF design, multi-layer PCB layout, embedded firmware development, and IoT database integration.

## System Architecture
* **Microcontroller:** ESP32-S3 (Dual-core, Wi-Fi / BLE enabled)
* **NFC Transceiver:** ST25R3916 (High output power, automated antenna tuning)
* **Antenna Design:** Custom planar loop antenna simulated in CST Studio Suite with a tuned LC matching network.
* **Peripherals:** I2C OLED display, status indicator LEDs, and buzzer feedback.

## Repository Structure
* `/hardware/kicad`: Multi-layer schematic and PCB layout files.
* `/hardware/cst_simulations`: 3D electromagnetic models and S-parameter extractions for the 13.56MHz antenna.
* `/firmware`: Embedded C++ application code running on the ESP32-S3.
* `/backend`: Local server and database scripts for logging inventory events.

## Getting Started
1. Clone the repository.
2. Open `/hardware/kicad/nfc-hub.kicad_pro` to inspect the schematic and layout.
3. Build the firmware using PlatformIO via `pio run`.
