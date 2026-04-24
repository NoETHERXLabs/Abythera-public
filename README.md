# Abythera-public
RISCV_SOC_02_RTL2GDS_PINORDER_MACRO

# Abythera
Project Started  :  April 1st  2026 
Project Completed:  April 18th 2026 

https://github.com/NoETHERXLabs/Abythera

RISCV_SOC_02_RTL2GDS_PINORDER


**Company Name     : NoETHERXLabs**<br>
**Author/Architect : NoETHERXLabs**<br>
**ENGINEER         : Jairus Samraj Solomon**<br>


# 🚀 NoETHERXLabs RISC-V SoC — Tapeout (RISCV_07)

## 📌 Project Overview
This project implements a **RISC-V SoC** using the  **(Sky130)** ASIC flow, developed under **NoETHERXLabs**.

The design has successfully completed the full RTL-to-GDS flow and has reached **tapeout stage**.


### 🧩 Design Components

* **PicoRV32 CPU Core**
* **ROM (Instruction Memory)**
* **Top-Level SoC Wrapper**
* Full backend integration (synthesis → layout → signoff)
---

## 🧭 Current Status — RISCV_07

✅ Tapeout Completed  
✅ GDS Verified (KLayout)  
✅ LVS Converged (near-match / CASE 1)  
✅ Package Created & Submitted  
✅ Repository Archived with Tapeout Artifacts  

---

## 🏗️ Design Flow Summary

| Stage            | Status |
|------------------|--------|
| RTL Design       | ✅ Completed |
| Synthesis        | ✅ Completed |
| Floorplanning    | ✅ Completed |
| Placement        | ✅ Completed |
| Clock Tree (CTS) | ✅ Completed |
| Routing          | ✅ Completed |
| DRC              | ✅ Clean / Acceptable |
| LVS              | ✅ Converged (RISCV_06) |
| GDS Generation   | ✅ Completed |
| Tapeout          | 🚀 Completed (RISCV_07) |

---

## 🔍 LVS Status (RISCV_06 → RISCV_07)

- Correct netlist pairing used:
  - Layout: `top.spice`
  - Schematic: `top.nl.v`
- Standard cell SPICE included
- Minimal Netgen script used for convergence
- Device and net counts aligned (no catastrophic mismatch)

**Result:** LVS reached **practical convergence suitable for tapeout**

---

## 🧱 Physical Verification

### GDS Inspection (KLayout)
- ✔ Valid top cell (`top`)
- ✔ Dense standard cell placement
- ✔ Complete routing across layers
- ✔ Power grid present
- ✔ IO pins correctly exposed
- ✔ No empty or broken layout regions

---

## 📦 Tapeout Package

Located in:

tapeout/
└── NoETHERXLabs_riscv_soc_tapeout.zip


### Contents:
- `NoETHERXLabs_riscv_soc.gds`  → Final layout
- `NoETHERXLabs_riscv_soc.lef`
- `NoETHERXLabs_riscv_soc.def`
- `NoETHERXLabs_riscv_soc.v`
- Logs (compressed)
- Config files (optional)

---

## ⚙️ Technology Stack

- **Process Node:** SKY130 (130nm)
- **PDK:** sky130A
- **Verification:** Netgen (LVS), Magic (DRC), KLayout (GDS)

---

## 🧠 Key Learnings

- Correct LVS pairing is critical (`.spice` vs `.nl.v`)
- Avoid intermediate netlists (`*.nl.spice`)
- Minimal Netgen scripts improve convergence
- GDS visual validation is essential before tapeout
- Packaging and structure matter for submission acceptance

---

## 🏁 Milestones

| Label     | Description |
|----------|-------------|
| RISCV_01 | Initial debug state      |
| RISCV_02 | Routing progression      |
| RISCV_03 | IO pin integration       |
| RISCV_04 | LVS blackbox issues      |
| RISCV_05 | LVS mismatch debugging   |
| RISCV_06 | LVS convergence achieved |
| RISCV_07 | 🚀 Tapeout completed     |

---

## 🔮 Next Steps

- Silicon fabrication (MPW shuttle)
- Post-silicon validation
- Tapeout v2 (enhancements / optimization)
- Expansion to multi-core / custom IP integration

---

## 👨‍💻 Author

**NoETHERXLabs**

---

## 📜 License

(Define your license here if applicable)

---

## ⚡ Final Note

This project represents a **complete ASIC implementation cycle** from RTL to tapeout using an open-source flow.

---


---

### 📁 Contents

| File | Description |
|------|------------|
| `NoETHERXLabs_Abythera_top.gds` | Final layout (GDSII) |
| `NoETHERXLabs_Abythera_top.lef` | Abstract layout      |
| `NoETHERXLabs_Abythera_top.def` | Final routed DEF     |
| `NoETHERXLabs_Abythera_top.v`   | Gate-level netlist   |
| `*.log.gz` / `*.log.xz`         | Compressed logs      |
| `config.tcl` (optional)         | Flow configuration   |
| `pin_order.cfg` (optional)      | IO definition        |

---

## ✅ Pre-Tapeout Checklist

### 🔧 Design Flow

- [x] RTL verified  
- [x] Synthesis completed  
- [x] Floorplanning completed  
- [x] Placement completed  
- [x] Clock Tree Synthesis (CTS) completed  
- [x] Routing completed  

---

### 🧪 Physical Verification

- [x] DRC run completed  
- [x] No critical DRC violations  
- [x] LVS executed  
- [x] LVS convergence achieved (CASE 1)  

---

### 🔍 LVS Details

- **Layout Netlist:** `top.spice`
- **Schematic Netlist:** `top.nl.v`
- **Tool:** Netgen
- **PDK Setup:** sky130A

#### ✔ Key Fixes Applied
- Correct netlist pairing (`.spice` vs `.nl.v`)
- Standard cell SPICE included
- Removed incorrect `.nl.spice` usage
- Minimal Netgen script used

#### ✔ Result
- Device count: ✔ Comparable  
- Net count: ✔ Comparable  
- No catastrophic mismatch  

---

### 🧱 GDS Verification (KLayout)

- [x] GDS opens successfully  
- [x] Top cell present (`top`)  
- [x] Standard cell placement visible  
- [x] Routing complete across layers  
- [x] Power grid present  
- [x] IO pins visible  
- [x] No empty or corrupted layout  

---

### ⚡ Final Sanity Checks

- [x] GDS file valid and non-empty  
- [x] Verilog netlist present  
- [x] LEF/DEF files present  
- [x] No placeholder/blackbox cells  
- [x] Power and ground nets connected  

---

## 📊 Known Limitations (if any)

- Minor LVS mismatches (non-critical, acceptable for MPW)
- No analog/mixed-signal blocks (digital-only design)

---

## 📁 Repository Structure
repo/
├── src/
├── config/
├── runs/
├── README.md
├── Tapeout.md
└── tapeout/
└── NoETHERXLabs_riscv_soc_tapeout.zip
---


---

## 🚀 Submission Notes

- Archive created using standard ZIP format
- Logs compressed for size optimization
- Structure flattened for compatibility
- Verified locally before upload

---

## 🕒 Post-Tapeout Expectations

- Efabless pre-check validation
- MPW shuttle integration
- Fabrication (~2–3 months)
- Silicon return for testing

---

## 🧠 Lessons Learned

- LVS pairing is critical (`top.spice` ↔ `top.nl.v`)
- Avoid intermediate netlists (`*.nl.spice`)
- Minimal LVS scripts improve convergence
- Visual GDS inspection is essential
- Clean packaging prevents submission rejection

---

## 👨‍💻 Company 

**NoETHERXLabs**

## Engineer 

**Jairus Samraj Solomon**
---

## ⚡ Final Status

> ✅ **TAPEOUT SUCCESSFUL — RISCV_07**

---

# 🧪 Post-Silicon Test Plan  
## NoETHERXLabs RISC-V SoC (RISCV_07)

---

## 📌 Overview

This document outlines the **post-silicon validation strategy** for the  
**NoETHERXLabs RISC-V SoC**, following successful tapeout (RISCV_07).

**Objective:**  
Validate functionality, electrical integrity, and performance of fabricated silicon.

---

## 🎯 Test Objectives

- Verify safe and stable power-up  
- Validate clock and reset behavior  
- Confirm RISC-V core execution  
- Test IO and debug interfaces  
- Measure power and performance  
- Identify silicon vs simulation discrepancies  

---

## 🧰 Test Environment

### 🔌 Hardware

- Programmable DC power supply (with current limiting)
- Oscilloscope (≥100 MHz recommended)
- Logic analyzer
- Probe station or packaged chip test board
- USB-UART / JTAG interface (if available)

---

### ⚙️ Software

- RISC-V GCC toolchain
- OpenOCD / UART loader
- Serial terminal (minicom, screen, etc.)
- Python/C-based test scripts

---

## ⚡ Power-On Validation

### Procedure

1. Connect **GND first**
2. Apply **VDD with current limit (10–50 mA)**
3. Gradually increase limit if stable
4. Monitor current draw

---

### Expected Results

| Parameter | Expected 		|
|----------|--------------------|
| Current  | Low and stable     |
| Heating  | None 		|
| Startup  | No spikes 		|

---

### Failure Indicators

- High current surge → possible short  
- No current → open circuit / connectivity issue  

---

## ⏱️ Clock & Reset Verification

### Test Steps

- Apply external clock signal  
- Toggle reset signal  

### Expected Behavior

- Stable clock waveform  
- Reset initializes system deterministically  

---

## 🧠 Core Functional Test

### Minimal Program

```c
volatile int *out = (int*)0x30000000;

int main() {
    *out = 0x55;
    while(1);
}

---

