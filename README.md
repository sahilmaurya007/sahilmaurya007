<div align="center">

<h2>Sahil Maurya</h2>

**Research Scholar · IIT Mandi, SCEE Department**<br>
*Digital VLSI Design · Post-Quantum Cryptography · RISC-V SoC Architecture*

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_LINKEDIN)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-4285F4?style=flat-square&logo=google-scholar&logoColor=white)](https://scholar.google.com/YOUR_PROFILE)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-00CCBB?style=flat-square&logo=researchgate&logoColor=white)](https://researchgate.net/profile/YOUR_PROFILE)
[![IIT Mandi](https://img.shields.io/badge/IIT%20Mandi-SCEE-darkblue?style=flat-square)](https://iitmandi.ac.in)
[![Email](https://img.shields.io/badge/Email-s22xxx@students.iitmandi.ac.in-red?style=flat-square&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL@students.iitmandi.ac.in)

</div>

---

## About

I am a Research Scholar at the **Indian Institute of Technology Mandi** (School of Computing and Electrical Engineering), conducting research at the intersection of **hardware security**, **digital VLSI**, and **post-quantum resilience**. My work focuses on the **hardware acceleration of lattice-based Post-Quantum Cryptographic (PQC) algorithms** — specifically CRYSTALS-Kyber and CRYSTALS-Dilithium — targeting both FPGA prototyping (Xilinx Vivado) and open-source ASIC tape-out flows (OpenLane + SkyWater 130nm PDK).

A key research objective is the **tight integration of PQC accelerator cores into RISC-V SoC platforms** via memory-mapped AXI-Lite peripherals, enabling post-quantum security in resource-constrained embedded and IoT systems without prohibitive area/power overhead.

My design methodology spans the full RTL-to-GDSII flow: RTL authoring in SystemVerilog → functional simulation (ModelSim/Icarus) → synthesis (Yosys/Vivado) → static timing analysis → place-and-route (OpenROAD) → DRC/LVS sign-off (Magic/Netgen).

> **Research Keywords:** RLWE · NTT · Polynomial Multiplication · Hardware Security · ASIC PPA Optimization · RISC-V Custom Extensions · Side-Channel Resistance

---

## Research Interests

| Domain | Topics |
|---|---|
| **Post-Quantum Cryptography** | CRYSTALS-Kyber (FIPS 203), CRYSTALS-Dilithium (FIPS 204), SPHINCS+, NTT-based polynomial multiplication, RLWE arithmetic |
| **Digital VLSI Design** | RTL design, synthesis optimization, static timing analysis (STA), design-for-testability (DFT), power-area-delay (PPA) tradeoffs |
| **RISC-V SoC Architecture** | RV32I/E pipeline design, custom ISA extensions, AXI4/AXI-Lite bus fabric, memory subsystem design |
| **Hardware Security** | Side-channel analysis countermeasures, masking schemes, DPA-resistant design, secure key storage |
| **Open-Source EDA** | OpenLane, OpenROAD, Yosys, SkyWater130nm PDK, Magic VLSI |

---

## Technology Stack

**Hardware Description & Verification**

![SystemVerilog](https://img.shields.io/badge/SystemVerilog-RTL%20Design-2563eb?style=flat-square)
![Verilog](https://img.shields.io/badge/Verilog-HDL-2563eb?style=flat-square)
![UVM](https://img.shields.io/badge/UVM-Verification-7c3aed?style=flat-square)
![VHDL](https://img.shields.io/badge/VHDL-Legacy%20IP-6b7280?style=flat-square)

**FPGA Tools**

![Vivado](https://img.shields.io/badge/Xilinx%20Vivado-2023.2-e11d48?style=flat-square)
![Quartus](https://img.shields.io/badge/Intel%20Quartus%20Prime-FPGA-0369a1?style=flat-square)
![ModelSim](https://img.shields.io/badge/ModelSim%2FQuesta-Simulation-16a34a?style=flat-square)
![GTKWave](https://img.shields.io/badge/GTKWave-Waveform%20Analysis-16a34a?style=flat-square)

**ASIC & Open-Source EDA**

![OpenLane](https://img.shields.io/badge/OpenLane-2.x-111827?style=flat-square)
![OpenROAD](https://img.shields.io/badge/OpenROAD-PnR-111827?style=flat-square)
![Yosys](https://img.shields.io/badge/Yosys-Synthesis-111827?style=flat-square)
![Magic](https://img.shields.io/badge/Magic%20VLSI-Layout%20%26%20DRC-111827?style=flat-square)
![SkyWater](https://img.shields.io/badge/SkyWater-130nm%20PDK-f59e0b?style=flat-square)
![Ngspice](https://img.shields.io/badge/Ngspice-Analog%20Sim-6b7280?style=flat-square)

**Scripting & Automation**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)
![TCL](https://img.shields.io/badge/TCL-EDA%20Scripting-0369a1?style=flat-square)
![Bash](https://img.shields.io/badge/Bash-Flow%20Automation-111827?style=flat-square)
![C](https://img.shields.io/badge/C-Embedded%20SW-gray?style=flat-square)

**Cryptographic Algorithms**

![Kyber](https://img.shields.io/badge/CRYSTALS--Kyber-FIPS%20203-7c3aed?style=flat-square)
![Dilithium](https://img.shields.io/badge/CRYSTALS--Dilithium-FIPS%20204-7c3aed?style=flat-square)
![AES](https://img.shields.io/badge/AES--256-Masking%20Impl.-6b7280?style=flat-square)
![SHA3](https://img.shields.io/badge/SHA3%2FSHAKE--256-Keccak%20Core-6b7280?style=flat-square)

---

## Featured Research Projects

<table>
<tr>
<th>Repository</th>
<th>Description</th>
<th>Tools</th>
<th>Status</th>
</tr>
<tr>
<td><a href="https://github.com/sahilmaurya007/kyber-ntt-hw-accelerator"><b>kyber-ntt-hw-accelerator</b></a></td>
<td>Area-time optimized hardware accelerator for CRYSTALS-Kyber KEM. Features pipelined NTT butterfly unit with RLWE modular multiplier. Taped out on SkyWater 130nm.</td>
<td>OpenLane · OpenROAD · SkyWater130</td>
<td>🟢 Active</td>
</tr>
<tr>
<td><a href="https://github.com/sahilmaurya007/riscv-pqc-soc"><b>riscv-pqc-soc</b></a></td>
<td>RISC-V (RV32I) SoC with memory-mapped PQC accelerator peripheral over AXI-Lite. Kyber-512 KEM executes in <5000 clock cycles on FPGA.</td>
<td>Vivado · PicoRV32 · AXI-Lite</td>
<td>🟢 Active</td>
</tr>
<tr>
<td><a href="https://github.com/sahilmaurya007/dilithium-signature-core"><b>dilithium-signature-core</b></a></td>
<td>Pipelined hardware core for CRYSTALS-Dilithium digital signature. Implements rejection sampling and polynomial arithmetic units.</td>
<td>Vivado · ModelSim · Yosys</td>
<td>🟡 In Progress</td>
</tr>
<tr>
<td><a href="https://github.com/sahilmaurya007/rlwe-modular-multiplier"><b>rlwe-modular-multiplier</b></a></td>
<td>High-speed modular multiplier targeting RLWE arithmetic (q=3329 for Kyber). NTT-friendly prime with Barrett reduction. Fully synthesizable RTL.</td>
<td>OpenLane · Yosys · GTKWave</td>
<td>🟢 Active</td>
</tr>
<tr>
<td><a href="https://github.com/sahilmaurya007/aes-masked-sbox"><b>aes-masked-sbox</b></a></td>
<td>First-order Boolean masked AES S-Box implementation resistant to DPA attacks. Verified against TVLA leakage detection methodology.</td>
<td>Vivado · ModelSim</td>
<td>🔵 Research</td>
</tr>
<tr>
<td><a href="https://github.com/sahilmaurya007/riscv-rv32i-pipeline"><b>riscv-rv32i-pipeline</b></a></td>
<td>5-stage pipelined RISC-V (RV32I) processor with hazard detection, data forwarding, and branch prediction. Verified against RISC-V compliance suite.</td>
<td>Vivado · GTKWave · OpenLane</td>
<td>🟢 Active</td>
</tr>
</table>

---

## Publications & Preprints

> *Placeholder — update as papers are accepted/published*

**Journal Articles (Under Review)**
- S. Maurya, [Advisor Name], "Area-Efficient NTT-Based Hardware Accelerator for CRYSTALS-Kyber on SkyWater 130nm CMOS," *IEEE Transactions on Very Large Scale Integration (VLSI) Systems*, 2025. *(under review)*

**Conference Papers**
- S. Maurya, [Advisor Name], "RISC-V SoC Integration of Post-Quantum Key Encapsulation Mechanism via AXI-Lite Peripheral," *IEEE International Symposium on Circuits and Systems (ISCAS)*, 2025. *(submitted)*

**Technical Reports**
- S. Maurya, "RLWE Modular Multiplier: RTL Design and OpenLane ASIC Flow on SkyWater 130nm," *IIT Mandi Technical Report*, 2024.

---

## Current Research Focus

```
Q1 2025 ──► Kyber NTT core — ASIC timing closure (SkyWater130, target: 100 MHz)
Q2 2025 ──► AXI-Lite peripheral wrapper, RISC-V SoC integration
Q3 2025 ──► Dilithium signature core — RTL complete, synthesis runs
Q4 2025 ──► IEEE TVLSI manuscript submission + FPGA demo (Artix-7)
```

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=sahilmaurya007&show_icons=true&theme=default&hide_border=true&count_private=true&include_all_commits=true)

</div>

---

<div align="center">
<sub><b>IIT Mandi · School of Computing and Electrical Engineering · Advanced Digital Systems Lab</b></sub><br>
<sub>Himachal Pradesh, India</sub>
</div>
