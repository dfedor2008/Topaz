

# Topaz - A Lightweight Long-Range GPS Telemetry System


---

## What is Topaz?

Topaz is a compact, cost-effective GPS telemetry platform designed for long-range data transmission using LoRa modulation. It supports both Morse code and binary telemetry formats and integrates environmental sensing, making it suitable for high-altitude ballooning, rocket recovery, remote monitoring, and more.

![Topaz In Action](https://github.com/user-attachments/assets/378aa5f3-1122-452e-8baf-344f799cf8b8)

---

## Features & Components

- **Microcontroller** — [ATSAMD21G18A](https://www.microchip.com/en-us/product/atsamd21g18): A reliable, low-power Cortex-M0+ MCU from Microchip.
- **LoRa Radio** — [SX1262](https://www.semtech.com/products/wireless-rf/lora-transceivers/sx1262): Sub-GHz long-range radio for Morse or telemetry data.
- **GPS Receiver** — [ATGM336H](https://jlcpcb.com/partdetail/Zhongkewei-ATGM336H5N31/C90770): Provides position and timing data.
- **Environmental Sensor** — [BME280](https://www.bosch-sensortec.com/products/environmental-sensors/humidity-sensors-bme280/): Measures temperature, humidity, and pressure.
- **Power Supply** — Designed to run from USB or external LiPo/boosted AA battery (3.3V).

---


---

## Use Cases

- Tracker for rockets
- Tracking for general uses
- Environmental monitoring (bme sensor)  

---

## How It Works

1. The **ATGM336H GPS module** gathers location and time.  
2. The **BME280** reads environmental parameters.  
3. The **SAMD21** processes the data.  
4. The **SX1262** transmits the payload via LoRa (in Morse or binary formats).  
5. A paired Topaz device or SDR can receive and decode the transmission.

All firmware is written in **C++**

---

## Hardware Setup Guide

1. **Solder the PCB** — A reflow plate is recommended for clean results.  
2. **Inspect for Shorts** — Pay extra attention around power and MCU pins.  
3. **Power Up via External Supply (not USB)** — Watch for smoke or abnormal heat. Power off immediately if detected.  
4. **Connect via USB** — Once verified safe, plug into your computer.

> After soldering and testing, upload the firmware via Arduino IDE. Topaz is optimized for affordability and robustness.

---

## PCB Diagrams

### Schematic

![Topaz Schematic](https://github.com/user-attachments/assets/f2879cd7-5488-43de-9e77-05d04c68f9a8)

### Layout

![Topaz Layout](https://github.com/user-attachments/assets/378aa5f3-1122-452e-8baf-344f799cf8b8)

---

## Software & Configuration

This project uses the Arduino platform. Libraries include:

- TinyGPS++  
- Adafruit_BME280  
- RadioHead or LoRa drivers for SX1262  




