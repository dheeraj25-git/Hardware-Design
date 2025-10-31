# 🎛️ **High-Performance Audio DSP System on Module (SoM)**  
### *Real-Time Mixed-Signal Platform for Modular Audio Processing*


## 🚀 **Overview**

A **compact, production-ready 40x40mm System on Module (SoM)** designed for **high-fidelity, real-time digital audio processing**. Built around the **STM32H7 (480 MHz Cortex-M7 + FPU/DSP)**, this modular platform enables **plug-and-play audio effects** (reverb, delay, distortion, EQ) via interchangeable **Daughterboards (Carrier Boards)**.

> **"Design once. Process everything."** 🎸🎤

---

## 🛠 **Tech Stack**

| Category              | Technology / Component                                 |
|-----------------------|--------------------------------------------------------|
| **MCU**               | STM32H743xI/G – 480 MHz, 2MB Flash, 1MB RAM, FPU + DSP |
| **Audio Codec**       | Integrated ADC/DAC + 4x SAI (Serial Audio Interface)   |
| **PCB**               | 4-Layer (Sig-GND-GND-Sig), Altium Designer             |
| **High-Speed I/O**    | 2x USB OTG HS/FS (crystal-less), 2x SDIO (125 MHz)     |
| **Power**             | 3.3V Digital + 1.8V Analog (isolated rails)            |
| **Debug**             | SWD via Tag-Connect (solderless), 24 MHz XTAL          |
| **Tools**             | STM32CubeIDE, STM32CubeMX                              |

---

## ✨ **Key Features**

- **Modular Mezzanine Interface**  
  → Reuse core SoM across guitar pedals, vocal processors, synths

- **Ultra-Low Noise Mixed-Signal Design**  
  - Physical **analog/digital separation**  
  - Pi-filter + ferrite beads on 1.8V analog rail  
  - 100 nF decoupling **per VDD/VBAT pin**

- **Pro-Grade Signal Integrity**  
  - Series resistor on SDIO CLK (EMI/ringing control)  
  - Dedicated **GND return per signal pin** on connector  
  - ESD-protected inputs + 2.2 kΩ I²C pull-ups

- **Real-Time DSP Engine**  
  - 480 MHz processing for **reverb, delay, overdrive, filters**  
  - Double-precision FPU + CMSIS-DSP optimized

---

## 📂 **Repository Structure**
