# Smart Soldering Iron (USB-C PD Powered)

A compact and affordable **USB-C PD powered smart soldering iron** designed for hobbyists and experimenters.
The project uses a **C210-style tip**, an **ATmega328P-AU**, and includes an **OLED display** and **accelerometer** for smart functions.

This repository currently contains **hardware-only KiCad files**. Firmware development will begin later.

---

## 📏 PCB Specifications

* **Size:** 15 mm × 107 mm
* **Layers:** 2-layer PCB
* **Form factor:** Ultra-slim to fit inside a pen-style soldering iron handle
* **Designed for:** C210-style soldering tip

---

## 🔌 Power System

* **Input:** USB-C Power Delivery
* **Supported Voltage:** Up to **12V** (currently limited to 12V for testing)
* **Purpose:** Drive the heater inside the C210 tip and power the MCU + peripherals

---

## 🧠 Microcontroller

* **MCU:** ATmega328P-AU
* **Package:** TQFP-32 (same package used in Arduino Uno SMD version)
* **Reason:** Easy programming, hobbyist-friendly, widely supported by Arduino IDE

---

## 🔥 Soldering Tip Support

* **Tip Type:** C210 series
* **Temperature Sensor:** Built-in thermocouple inside the tip
* **Connection:** Compact, high-current heater + thermocouple feedback

---

## 📟 Display & User Interface

* **Display:** 128×32 OLED
* **Navigation:** Buttons + planned touch navigation for PDF schematic viewing
* **Future UI Features:**

  * Temperature selection menu
  * Left-hand / right-hand screen rotation
  * Real-time tip temperature graph (optional)

---

## 🧭 Motion / Sleep Features

* **Accelerometer:** LIS3DHTR
* Planned features:

  * Auto-sleep when inactive
  * Wake-on-shake
  * Handle movement detection for safety

---

## 🧪 Project Status

| Category   | Status                        |
| ---------- | ----------------------------- |
| Hardware   | ✔ Completed (prototype ready) |
| Schematics | ✔ Completed                   |
| PCB Layout | ✔ Completed                   |
| Firmware   | ❌ Not started                 |
| Testing    | ❌ Pending                     |

---

## 🧰 Development Plans (Firmware)

Firmware will be written primarily using **Arduino IDE**, with possible low-level C enhancements.

Planned firmware features:

* PID temperature control
* USB-C PD negotiation and power step handling
* On-screen temperature display
* Menu navigation
* Accelerometer-based sleep mode
* Tip calibration

---

## 📂 Repository Structure

* `.kicad_pro` – Main KiCad project file
* `.kicad_sch` – Schematic files
* `.kicad_pcb` – PCB layout
* `pcb_front.pdf` / `pcb_back.pdf` – PDF views of the PCB
* Additional supporting schematic sheets

Touch navigation support will be added to PDF schematics to improve readability during review.

---

## 🎯 Project Goal

To create an **affordable**, **compact**, and **easily buildable** smart soldering iron that:

* Hobbyists can assemble with basic tools
* Works reliably with USB-C PD chargers
* Uses a high-quality C210 tip
* Provides a solid foundation for firmware experimentation

---

## 📜 License

No license added yet — you may add MIT / GPL / CERN OHL based on your preference.

---

## 🤝 Contributions

Contributions and suggestions are welcome once firmware development begins!
