# GreenHAir Node

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-Development-orange.svg)](https://github.com/username/repo)
[![KiCad](https://img.shields.io/badge/EDA-KiCad_9.0-purple)](https://www.kicad.org/)

A Bluetooth Low Energy (BLE) Node based on the Nordic Semiconductor nRF54L series. Designed for environmental monitoring and efficient data transmission.

## Features

*   **Core:** Powered by the Nordic nRF54L series for ultra-low power consumption.
*   **Connectivity:** Bluetooth Low Energy (BLE) for reliable wireless communication.
*   **Modular Design:** Separate schematics for MCU, PSU, and Sensors for easy customization.
*   **Power Supply:** Optimized power management unit (`psu.kicad_sch`) powered by a CR2032 coin cell.
*   **Sensing:** Equipped with an AS7341DLG Lux sensor (I2C) for precise light measurement (`sensor.kicad_sch`).
*   **RF Performance:** Includes various antenna footprint options for optimal range.

## Hardware Structure

The project is divided into several KiCad schematics:

*   `GreenHAir_Node.kicad_sch`: Top-level hierarchy.
*   `mcu.kicad_sch`: Microcontroller and core logic.
*   `psu.kicad_sch`: Power supply and management.
*   `sensor.kicad_sch`: Sensor interfaces and components.

## Installation & Fabrication

### 1. PCB Fabrication
Generate the Gerber files from `GreenHAir_Node.kicad_pcb` and send them to your preferred PCB manufacturer.

### 2. Assembly
Follow the BOM (Bill of Materials) generated from the schematic to source and solder components.

### 3. Firmware
(Add instructions for flashing the nRF54L chip here)

## Customization

### Sensors
Currently populated with an AS7341DLG spectral sensor. The `sensor.kicad_sch` sheet allows for easy modification or expansion of the sensor array.

### Antenna
The design supports multiple antenna configurations found in the `libs/RF_Antenna.pretty` library.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1.  Fork the repository
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.