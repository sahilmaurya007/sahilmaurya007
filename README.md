<!-- 
====================================================================================================
RESEARCHER PROFILE: SAHIL MAURYA (IIT MANDI)
====================================================================================================
-->

<div align="center">

# 🚀 Sahil Maurya
### **Research Scholar @ IIT Mandi | Digital VLSI | PQC Architect | RISC-V SoC Developer**

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=36BCF7&center=true&vCenter=true&width=600&lines=Building+Secure+Hardware+for+a+Post-Quantum+World;Researching+Lattice-based+Cryptography+Accelerators;Developing+Energy-Efficient+Neuromorphic+SoCs;Expert+in+FPGA+%26+ASIC+Design+Flows)](https://git.io/typing-svg)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,70:003366,100:000000&height=250&section=header&text=VLSI%20%7C%20PQC%20%7C%20RISC-V&fontSize=50&animation=fadeIn&fontAlignY=35" width="100%" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Research-IIT%20Mandi-blue?style=for-the-badge&logo=icloud&logoColor=white" />
  <img src="https://img.shields.io/badge/VLSI-Digital%20Design-orange?style=for-the-badge&logo=micro-strategy&logoColor=white" />
  <img src="https://img.shields.io/badge/Security-Post%20Quantum-red?style=for-the-badge&logo=securityscorecard&logoColor=white" />
  <img src="https://img.shields.io/badge/RISC--V-SoC%20Architect-green?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---

## 👨‍🔬 Research Vision & Objective
> *"My research focuses on the hardware-software co-design of secure, high-performance cryptographic accelerators. By bridging the gap between mathematical complexity and silicon efficiency, I aim to develop RISC-V based SoCs that are resilient against the computational might of future quantum computers."*

</div>

---

## 🏛️ Academic Pedigree

<table width="100%">
  <tr>
    <th width="20%">Degree</th>
    <th width="40%">Institution</th>
    <th width="20%">Status/Year</th>
    <th width="20%">PPA/CGPA</th>
  </tr>
  <tr>
    <td><b>Research Scholar (Ph.D.)</b></td>
    <td>Indian Institute of Technology (IIT), Mandi</td>
    <td>2025 - Present</td>
    <td>8.33/10.0</td>
  </tr>
  <tr>
    <td><b>M.Tech (VLSI & Embedded)</b></td>
    <td>Indian Institute of Information Technology (IIIT), Guwahati</td>
    <td>2021 - 2023</td>
    <td>9.11/10.0 (Gold Medalist)</td>
  </tr>
  <tr>
    <td><b>B.Tech (ECE)</b></td>
    <td>University of Lucknow, Uttar Pradesh</td>
    <td>2017 - 2021</td>
    <td>66.1%</td>
  </tr>
</table>

---

## 🛠️ Comprehensive Technical Stack

### **Hardware Description & Verification**
<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=verilog,cpp,py,matlab,linux,git,github,bash,ubuntu,vscode,visualstudio" />
  </a>
</p>

| **Category** | **Specific Tools & Expertise** |
| :--- | :--- |
| **EDA Toolchain** | Xilinx Vivado ML, Vitis HLS, Vitis AI, Cadence Genus, Innovus, Xcelium, ModelSim, Questasim |
| **ASIC Flows** | OpenLane, OpenROAD, SkyWater 130nm, Magic VLSI, Netgen, KLayout, STA (Tempus) |
| **FPGA Prototyping** | Zynq UltraScale+ (ZCU102), Kintex-7, Artix-7, Zynq-7000 (Zybo Z7, ZedBoard) |
| **Protocols & Interconnects** | AMBA AXI4 (Full, Lite, Stream), APB, AHB, I2C, SPI, UART, PCIe (Basics) |
| **Cryptographic Primitives** | NTT (Number Theoretic Transform), Montgomery Multipliers, Keccak (SHA-3), AES-GCM |

---

## 📚 Selected Research Publications
<details open>
<summary><b>View Research Impact (IEEE Style)</b></summary>

1. **S. Maurya**, "Neuromorphic Adaptive Precision RISC-V Processor with Real-Time Precision Scaling and Neuronal State Management," *Accepted at IEEE International Conference on High Performance Computing (HiPC)*, 2025.
2. **S. Maurya**, "Approximate Modular Multipliers for R-LWE Cryptosystems on FPGAs and ASICs," *Published in IEEE SILCON*, 2024.
3. [Working Paper] "Energy-Efficient NTT Hardware Accelerator for crystals-kyber targeting Resource-Constrained IoT Devices."
4. [Working Paper] "Lattice-based Digital Signature Acceleration on RISC-V Vector Extensions."

</details>

---

## 🚀 Research-Grade Projects Ecosystem

### **1. Secure RISC-V SoC with Integrated PQC (Kyber-SoC)**
*   **Problem**: Post-Quantum Cryptography (PQC) is computationally too heavy for general-purpose RISC-V cores.
*   **Architecture**: A decoupled 5-stage RV32I pipeline with a custom AXI4-Stream interface to a hardware NTT-accelerator.
*   **Tools**: Vivado 2024.2, OpenLane.
*   **Key Results**: 12x reduction in clock cycles for Kyber-768 key encapsulation compared to pure software.
*   **Research Potential**: Implementation of side-channel masking techniques.

### **2. AxMM-RLWE: Approximate Modular Multiplier**
*   **Problem**: Precise modular multiplication consumes excessive area and power in lightweight crypto.
*   **Architecture**: Design of an Error-Configurable Approximate Modular Multiplier (AxMM) using 45nm Nangate ASIC.
*   **Metrics**: 18% Power reduction, 22% Area reduction with <0.5% error probability.
*   **Status**: Published in IEEE SILCON 2024.

### **3. Neuromorphic Adaptive Precision Unit (NAPU)**
*   **Problem**: Static precision in SNNs (Spiking Neural Networks) leads to energy wastage.
*   **Architecture**: A real-time precision scaling unit that adjusts bit-width based on neuronal activity.
*   **Tools**: Vitis HLS, Vivado.
*   **Status**: Accepted at HiPC 2025.

### **4. Side-Channel Analysis (SCA) Sandbox**
*   **Problem**: Difficulty in evaluating power leakage without expensive oscilloscopes.
*   **Architecture**: FPGA-based power simulation framework using switching activity logs (SAIF/VCD).
*   **Tools**: Cadence Joules, Xilinx Power Analyzer.

### **5. Hardware-Accelerated NTT butterfly for CRYSTALS-Kyber**
*   **Architecture**: Radix-2 Decimation-in-Time (DIT) NTT unit with multi-bank memory for conflict-free access.
*   **Results**: Throughput of 1024 points/cycle at 250MHz on ZCU102.

### **6. PUF-based Secure Key Storage (KMU)**
*   **Architecture**: Physically Unclonable Function (PUF) integrated into the RISC-V bootloader sequence.

---

## 🛠️ Full Implementation Deep-Dive

### **Project A: High-Throughput NTT Accelerator**
**RTL Structure**:
```text
ntt_core/
├── rtl/
│   ├── butterfly_unit.v       # Dual-path modular arithmetic
│   ├── address_generator.v    # Bit-reversal and stride logic
│   ├── memory_controller.v    # Multi-bank SRAM interface
│   └── ntt_top.v              # FSM and control logic
├── tb/
│   ├── ntt_tb.sv              # SystemVerilog testbench
│   └── ntt_vectors.txt        # Golden vectors from Python
└── scripts/
    └── synth.tcl              # Vivado synthesis script
```
**Synthesis Results (Target: ZCU102)**:
- **LUTs**: 4,200 (2.5% usage)
- **DSPs**: 12 (Montgomery Multipliers)
- **Max Freq**: 320 MHz
- **Timing Slack**: +1.24ns

### **Project B: Secure RISC-V SoC (RV32I_Secure)**
**Architecture**:
- **Pipeline**: 5-stage (IF, ID, EX, MEM, WB).
- **Security**: Hardware-enforced stack protection and encrypted instruction memory.
- **ASIC Flow**: GDSII generated using OpenLane (Sky130).
- **PPA Report**: Area = 0.45mm², Power = 12mW @ 100MHz.

---

## 🏗️ PQC + RISC-V Integration (Advanced)
<div align="center">
  <img src="https://raw.githubusercontent.com/sahilmaurya007/sahilmaurya007/main/soc_arch.png" width="80%" alt="SoC Architecture Diagram" />
  <br>
  <i>Conceptual Architecture: RV32I Core with PQC Coprocessor over AXI Interconnect</i>
</div>

- **Memory Mapping**:
  - `0x4000_0000`: PQC Control Register (Start, Reset, Interrupt Enable).
  - `0x4000_0004`: PQC Status Register (Busy, Done, Error).
  - `0x4000_1000 - 0x4000_1FFF`: Shared Buffer for Polynomial Coefficients.
- **Instruction Flow**:
  1. RISC-V writes data to Shared Buffer.
  2. RISC-V writes `1` to `Control Register`.
  3. PQC Coprocessor executes NTT/PWM.
  4. PQC raises an interrupt or sets `Done` flag.
  5. RISC-V reads results.

---

## 📈 Profile Strength & Strategy
To maintain a high-impact GitHub profile, I follow these principles:
- **Daily Commits**: Pushing incremental updates to RTL modules or synthesis reports.
- **Documentation**: Every repository includes a `README.md` with PPA results and architecture diagrams.
- **Active Verification**: Using CI/CD pipelines to run testbenches on every push.
- **Open Science**: Sharing Python-based golden models used for hardware verification.

---

## 📊 Dynamic Stats & Analytics
<p align="center">
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=sahilmaurya007&show_icons=true&theme=tokyonight&count_private=true&hide_border=true" />
  <img width="48%" src="https://github-readme-streak-stats.herokuapp.com/?user=sahilmaurya007&theme=tokyonight&hide_border=true" />
</p>

<p align="center">
  <img width="100%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sahilmaurya007&layout=compact&theme=tokyonight&hide_border=true" />
</p>

---

## 📫 Connect with Me
- 📧 **Email**: [d24204@students.iitmandi.ac.in](mailto:d24204@students.iitmandi.ac.in)
- 💼 **LinkedIn**: [sahilmaurya007](https://linkedin.com/in/sahilmaurya007)
- 🎓 **Google Scholar**: [Sahil Maurya](https://scholar.google.com)
- 📍 **Office**: SCEE Department, IIT Mandi, Himachal Pradesh.

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=sahilmaurya007&color=blueviolet" alt="Profile Views" />
  <br>
  <sub>© 2026 Sahil Maurya | Research & Innovation | Digital VLSI | PQC | RISC-V</sub>
</div>
