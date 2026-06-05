# 🛰️ RikAgriculture-Pro: Pulse Sentinel & Seasonal Advisors

An ultra-low-cost (~₹450), value-engineered off-grid crop defense edge architecture integrated with seasonal, trilingual crop advisor web modules (English, Hindi, Bengali).

---

## 🌾 Project Overview

This ecosystem combines standalone physical boundary security with digital seasonal diagnostics to protect and optimize smallholder agricultural plots. 

### 🌟 Key Features
* **Anti-Habituation Engine:** Uses true random seeds via a floating analog pin to fluctuate sound sweeps (2kHz - 12kHz) and optic strobes.
* **Ultra-Low Power Standby:** Engineered to minimize parasitic draw by removing the onboard power SMD LED from the MCU.
* **Kharif Season Portal:** Interactive diagnostics for monsoon crops including Paddy/Rice, Cotton, and Groundnut.
* **Rabi Season Portal:** Interactive winter crop matrix tracking Wheat, Mustard, and Chickpea.

---

## 🛠️ Hardware Architecture & Pin Mapping

### Component Breakdown (BOM < ₹500)
* **MCU:** Arduino Pro Mini (3.3V / 8MHz)
* **Acoustic:** High-Decibel Piezo Buzzer
* **Optic:** 1W White LED + BC547 NPN Transistor
* **Power:** Recycled 18650 Li-Ion Cell + 5V (100mA) Epoxy Solar Panel
* **Enclosure:** IP65 Waterproof PVC Junction Box

### Pin Connections


| Component | Arduino Pro Mini Pin | Description |
| :--- | :--- | :--- |
| **Piezo Buzzer (+)** | `D9` | Generates randomized audio frequency sweeps |
| **Transistor Base (BC547)** | `D10` | Controls high-intensity 1W LED strobe cycles |
| **Floating Seed Pin** | `A0` | Left open to generate random visual/audio timing |

---

## 📂 Repository Structure

```text
├── Firmware/
│   └── Sentinel_Core.ino   # Arduino C++ edge firmware script
├── Web/
│   ├── sentinel.html       # Mobile-friendly trilingual crop defense portal
│   ├── kharif.html         # Kharif Season Advisor (Paddy, Cotton, Groundnut)
│   └── rabi.html           # Rabi Season Advisor (Wheat, Mustard, Chickpea)
└── README.md               # Project documentation core
```

---

## 🚀 Deployment Best Practices

1. **Hardware Power Trick:** Desolder the default internal power LED on your Arduino Pro Mini. This reduces passive standby current down into micro-amperes to maximize 18650 lifecycle longevity.
2. **Rain Safeguard:** When drilling the acoustic sound escape port on your IP65 junction box, ensure it is positioned strictly on the bottom face to keep tropical downpours from pooling inside.

---

## 👥 Author
* **Rik** - Lead Architect & Developer at RikMakersHub
