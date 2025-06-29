# Topaz

**Topaz** is a low-cost, long-range GPS telemetry system based on a custom PCB. It uses an **SX1262 LoRa radio** to send **Morse code** or **telemetry data** up to 13 km. It can also transmit **temperature, pressure, and humidity** using a BME280 sensor.

---

## Overview

- **Microcontroller**: SAMD21 — chosen for reliability and familiarity.
- **Radio**: SX1262 — supports long-range communication using LoRa.
- **Sensor**: BME280 — measures temperature, humidity, and barometric pressure.
- **GPS**: ATGM336H — provides real-time location and telemetry data.

---

## Why I Made This Project

I originally built Topaz as a personal **GPS tracker** to monitor my frequently late bus. Later, I realized it could also be used for fun applications—like tracking my brother during a game of hide and seek!

This idea quickly expanded into a general-purpose tracking system that can be used for many projects involving remote data transmission.

---

## Use Cases

Topaz can be used in a variety of real-world and hobbyist applications:

- Tracking hikers or groups in remote areas  
- Recovery of rockets or weather balloons  
- Monitoring environmental conditions  
- Custom telemetry projects without relying on cellular networks

---

## How It Works

1. The **ATGM336H GPS module** collects location and telemetry data.  
2. The **SAMD21** processes the data and controls device operation.  
3. The **SX1262 LoRa module** transmits the data in Morse code or as packets.  
4. A second Topaz device can act as a **receiver**, enabling two-way communication.

All code is written in **C++** using well-supported sensor libraries.

---

## Application Notes

After receiving the PCB:

1. **Solder the board** — a heating plate is recommended if you have one.  
2. **Inspect for shorts** — especially around the microcontroller and power lines.  
3. **Power the board (not via computer USB yet)** — if you see smoke, **unplug immediately** and re-check the solder joints.  
4. Once no shorts are found, plug into your computer via USB.

> 🔧 The firmware will be uploaded after PCB assembly. The entire design is optimized for **low cost** and **reliability**.

---

## PCB Schematic

![Topaz Schematic](https://github.com/user-attachments/assets/f2879cd7-5488-43de-9e77-05d04c68f9a8)

---

## PCB Layout

![Topaz Layout](https://github.com/user-attachments/assets/378aa5f3-1122-452e-8baf-344f799cf8b8)






