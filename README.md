# Sahil Maurya

**Research Scholar** | School of Computing & Electrical Engineering (SCEE)  
**Indian Institute of Technology Mandi** | **A²DSL Lab**

I design **secure and efficient hardware accelerators** for Post-Quantum Cryptography (PQC) using advanced Digital VLSI and RISC-V SoC techniques. My focus lies in RTL-to-GDSII implementation of NIST PQC algorithms (Kyber/ML-KEM, Dilithium/ML-DSA) with emphasis on high-throughput NTT, modular arithmetic, side-channel resistance, and low-power optimization on both FPGA and ASIC platforms.

[![GitHub followers](https://img.shields.io/github/followers/sahilmaurya007?style=social)](https://github.com/sahilmaurya007)
[![Google Scholar](https://img.shields.io/badge/Google_Scholar-Profile-4285F4)](https://scholar.google.com/citations?user=your-id)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2)](https://www.linkedin.com/in/sahilmaurya007)
[![ORCID](https://img.shields.io/badge/ORCID-0000-0000-0000-0000-blue)](https://orcid.org/)

---

## Research Interests

- **Post-Quantum Cryptography Hardware**: Acceleration of lattice-based schemes (RLWE, NTT, Gaussian sampling) with side-channel protection.
- **Digital VLSI Design**: RTL design, synthesis, STA, low-power techniques, DFT, and full ASIC flow (OpenLane / Sky130).
- **RISC-V SoC Development**: Custom cryptographic extensions and AXI4/APB integration for secure processors.

---

## Tech Stack

**HDL & Languages**  
![Verilog](https://img.shields.io/badge/Verilog-1E90FF?logo=verilog&logoColor=white) 
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-FF4500) 
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) 
![TCL](https://img.shields.io/badge/TCL-1E90FF)

**EDA & Implementation Tools**  
![Vivado](https://img.shields.io/badge/Vivado-FF0000?logo=xilinx&logoColor=white) 
![OpenLane](https://img.shields.io/badge/OpenLane-00A0B0) 
![OpenROAD](https://img.shields.io/badge/OpenROAD-00A0B0) 
![Yosys](https://img.shields.io/badge/Yosys-00A0B0) 
![GTKWave](https://img.shields.io/badge/GTKWave-1E90FF)

**Domains**  
![PQC](https://img.shields.io/badge/PQC-Post--Quantum_Cryptography-8A2BE2) 
![RISC--V](https://img.shields.io/badge/RISC--V-Architecture-228B22) 
![ASIC](https://img.shields.io/badge/ASIC-Full_Flow-FF4500) 
![FPGA](https://img.shields.io/badge/FPGA-Prototyping-00BFFF)

---

## Featured Research Projects

All projects follow a professional repository structure (`rtl/`, `tb/`, `scripts/`, `synthesis/`, `docs/`, `results/`) and are designed for direct IEEE publication potential. They build on my hands-on experience with RLWE modular multipliers, Vivado, and OpenLane flows.

| # | Repository | Domain | Key Highlights | Status |
|---|------------|--------|----------------|--------|
| 1 | [rlwe-modular-multiplier-pqc](https://github.com/sahilmaurya007/rlwe-modular-multiplier-pqc) | PQC Acceleration | 4-stage pipelined Montgomery + Barrett reduction; 2.1× throughput | FPGA + OpenLane ASIC |
| 2 | [kyber-ntt-accelerator](https://github.com/sahilmaurya007/kyber-ntt-accelerator) | PQC (Kyber) | 512-point radix-2 NTT; 1.2 µs latency, clock-gated | Vivado + OpenLane |
| 3 | [riscv-pqc-coprocessor](https://github.com/sahilmaurya007/riscv-pqc-coprocessor) | RISC-V + PQC | RV32I with custom PQC instructions + AXI4 integration | Full SoC (FPGA/ASIC) |
| 4 | [dilithium-gaussian-sampler-asic](https://github.com/sahilmaurya007/dilithium-gaussian-sampler-asic) | Digital VLSI + PQC | Constant-time CDT/Knuth-Yao sampler in Sky130 PDK | OpenLane GDSII ready |
| 5 | [axi-crypto-interconnect](https://github.com/sahilmaurya007/axi-crypto-interconnect) | RISC-V SoC | 4-master AXI4 crossbar for multiple PQC IPs | Vivado block design |
| 6 | [lowpower-ntt-vlsi](https://github.com/sahilmaurya007/lowpower-ntt-vlsi) | Digital VLSI | Fine-grained clock gating; 35% dynamic power reduction | Synopsys / OpenLane |
| 7 | [sidechannel-resistant-kyber](https://github.com/sahilmaurya007/sidechannel-resistant-kyber) | PQC Security | Masked arithmetic NTT with dual-rail logic | FPGA + leakage analysis |
| 8 | [riscv-pqc-secure-soc](https://github.com/sahilmaurya007/riscv-pqc-secure-soc) | Advanced SoC | Complete RISC-V SoC with integrated PQC coprocessor | Bootable on FPGA |

**Repository Standards**: Each repo contains synthesizable Verilog, comprehensive testbenches, synthesis/STA reports, power analysis, GTKWave screenshots, and a detailed professional README with PPA metrics (LUTs, power, delay, area).

---

## Publications

- S. Maurya et al., “Hardware Acceleration of RLWE-Based Modular Multiplication for CRYSTALS-Kyber on FPGA and ASIC,” *IEEE Transactions on Circuits and Systems I* (under review).  
- S. Maurya et al., “A RISC-V SoC with Integrated Post-Quantum Cryptographic Coprocessor using OpenLane Flow,” *IEEE International Symposium on Circuits and Systems (ISCAS)*, 2026 (targeted).

(Google Scholar and arXiv links will be updated upon acceptance)

---

## 📫 Get in Touch

- **Email**: [your.email@iitmandi.ac.in](mailto:your.email@iitmandi.ac.in)  
- **Lab**: [A²DSL Lab, SCEE, IIT Mandi](https://www.iitmandi.ac.in)  
- **Location**: Kamand Campus, Mandi, Himachal Pradesh, India  

*"Building trustworthy hardware for the post-quantum era."*

---

**Last Updated**: March 2026  
All repositories are actively maintained with regular commits of RTL updates, synthesis results, and documentation.
