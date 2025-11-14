# STRF blueMoon — USB to 2.4 GHz nRF24L01+ Wireless Transceiver Dongle

*Compact USB-powered 2.4 GHz RF dongle with STM32 + nRF24L01+ for wireless serial, IoT, and RC applications.*

---

## Overview

**STRF** is a custom-designed USB-to-2.4GHz RF bridge combining:
- **STM32F0xx** microcontroller (LQFP32)
- **nRF24L01+** 2.4 GHz ISM band transceiver
- **SMA connector** for external antenna
- **SWD debug header**
- **USB Type-B plug** for power and data

Designed in **KiCad 9.0.1**, this board enables **wireless serial communication**, **packet sniffing**, or **IoT gateway** functionality from any USB host (PC, Raspberry Pi, etc.).

---

## Features

| Feature | Specification |
|-------|---------------|
| **MCU** | STM32F0 series |
| **RF Chip** | nRF24L01+ (2.4 GHz, 250 kbps – 2 Mbps) |
| **Interface** | USB 2.0 Full-Speed (Virtual COM Port) |
| **Antenna Port** | SMA female (50 Ω) |
| **Debug** | SWD (SWDIO, SWCLK, NRST, 3.3V, GND) |
| **Power** | USB-powered (5V → 3.3V LDO) |
| **Dimensions** | **38.25 mm × 15.75 mm** |
| **PCB Layers** | 4-layer FR4 |

---

## Block Diagram

```text
[USB Host] ←USB→ [STM32F0] ←SPI→ [nRF24L01+] ←RF→ [SMA Antenna]
                    ↑
                 [SWD Debug]
