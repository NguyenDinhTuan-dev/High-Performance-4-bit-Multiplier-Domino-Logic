# High-Performance 4-Bit Multiplier: UT Algorithm & Domino Logic

![Cadence](https://img.shields.io/badge/Tool-Cadence%20Virtuoso-black?style=flat-square&logo=cadence)
![Technology](https://img.shields.io/badge/Tech-90nm%20CMOS-blue?style=flat-square)
![Type](https://img.shields.io/badge/Type-Course%20Project-green?style=flat-square)

## 📖 Project Overview
This project presents the design and transistor-level simulation of a **4-Bit Multiplier** aimed at high-speed processing. The design leverages the **Urdhva Tiryagbhyam (UT)** algorithm from Vedic Mathematics to reduce partial products and employs **Domino Logic** to minimize critical path delays.

The primary goal was to compare the dynamic performance and power consumption against a standard Static CMOS baseline using **90nm CMOS technology**.

## ⚙️ Design Specifications
### 1. Algorithm: Urdhva Tiryagbhyam (UT)
* Utilizes the "Vertically and Crosswise" method.
* Significantly reduces logic depth compared to conventional Array or Booth multipliers.

### 2. Logic Families Implementation
* **Static CMOS (Baseline):** Implemented using standard PUN/PDN networks for power/delay benchmarking.
* **Domino Logic (Proposed):** Utilizes dynamic logic with separate *Precharge* and *Evaluation* phases to achieve faster switching speeds.

### 3. Key Components
* Logic Gates: NOT, AND, OR, XOR.
* Arithmetic Units: Half Adders, Full Adders, 4-bit Ripple Carry Adders (RCA).
* **Technology Node:** 90nm CMOS Process.

## 🛠 Tools & Environment
* **Schematic Entry & Simulation:** Cadence Virtuoso.
* **Waveform Analysis:** Virtuoso Visualization & Analysis (Viva).
* **Data Processing:** Microsoft Excel (Delay & Power comparative analysis).

## 📂 Repository Contents
The design files are archived based on the logic family:

* 📁 **`Static_CMOS.rar`**: Complete schematic and simulation states for the standard CMOS design.
* 📁 **`Domino_CMOS.rar`**: Complete schematic and simulation states for the high-speed Domino Logic design.

*(Note: Download the .rar files and extract them to view the Cadence libraries)*

## 📊 Performance Analysis
The following table summarizes the simulation results comparing the two architectures:

| Metric | Static CMOS | Domino Logic | Analysis |
| :--- | :--- | :--- | :--- |
| **Delay (Speed)** | Baseline | **27% Faster** | Domino logic significantly optimizes critical path timing. |
| **Static Power** | Lower | **+4% Higher** | Minor increase in leakage due to dynamic circuitry. |
| **Dynamic Power** | Lower | **+21% Higher** | Higher switching activity leads to increased dynamic power consumption. |

> **Conclusion:** While Domino Logic consumes more power due to the clock distribution and switching activity, it offers a superior speed advantage (**27% improvement**), making it ideal for high-performance Arithmetic Logic Units (ALUs) where speed is the priority.

## 📜 References
1.  N. L. Reddy et al., *"Design of a high performance 4 bit multiplier using UT algorithm with domino logic,"* IEMCON 2016.
2.  Course Project Report: *High Performance 4 Bit Multiplier Using UT Algorithm With Domino Logic*, HCMUTE, Jan 2025.

---
<p align="center">
  <i>Developed by Nguyen Dinh Tuan & Team</i>
</p>
