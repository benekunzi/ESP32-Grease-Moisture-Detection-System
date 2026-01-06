# ESP32 Grease Moisture Detection System

This repository contains the firmware for a research project at **OVGU** focused on detecting moisture content in grease using precision capacitance measurements.

## Project Overview

The system utilizes an ESP32 microcontroller to measure the charging time of capacitors formed within grease samples. By analyzing the capacitance changes, the moisture level in the grease can be estimated.

## Key Features

- **Precision Timing**: High-resolution measurement of capacitor charging times.
- **Capacitance Measurement**: Calculates capacitance (CM and CREF) based on charging curves.
- **Signal Processing**: Implements a median filter to reduce noise in measurements.
- **Programming Language**: Developed using **C**.
- **ESP-IDF Framework**: Built using the Espressif IoT Development Framework.

## Hardware Components

- **MCU**: ESP32 (DevKit)
- **Pins**:
  - `GPIO 32/33`: Charging control outputs.
  - `GPIO 34/35`: ADC inputs for voltage level monitoring.
  - `GPIO 25/26`: Interrupt inputs for timing capture.

## Setup and Build

This project is configured for use with **PlatformIO**.

1.  Install [PlatformIO IDE](https://platformio.org/platformio-ide).
2.  Clone this repository.
3.  Open the project in PlatformIO.
4.  Build and upload to your ESP32.

```bash
# Optional: CLI build
pio run -t upload
```

## Authors

Developed as part of a research project at Otto-von-Guericke-Universität Magdeburg (OVGU).
