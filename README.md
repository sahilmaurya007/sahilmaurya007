<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Sahil Maurya | PQC Hardware Architect | IIT Mandi</title>
  <!-- Google Fonts & Material Icons -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #05070f;
      font-family: 'Inter', sans-serif;
      color: #eef5ff;
      line-height: 1.5;
      scroll-behavior: smooth;
      overflow-x: hidden;
    }

    /* animated mesh gradient background */
    .bg-orb {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -2;
      background: radial-gradient(circle at 20% 30%, #0a0f2a, #010103);
      overflow: hidden;
    }

    .bg-orb::before,
    .bg-orb::after {
      content: "";
      position: absolute;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle at 70% 80%, rgba(0, 212, 255, 0.08), transparent 70%);
      animation: drift 28s infinite alternate;
    }

    .bg-orb::after {
      background: radial-gradient(circle at 20% 20%, rgba(100, 70, 200, 0.1), transparent 60%);
      animation: drift 35s infinite alternate-reverse;
    }

    @keyframes drift {
      0% { transform: translate(0%, 0%) scale(1); opacity: 0.4; }
      100% { transform: translate(5%, 8%) scale(1.2); opacity: 0.8; }
    }

    /* glassmorphic card style */
    .glass-card {
      background: rgba(10, 20, 35, 0.5);
      backdrop-filter: blur(12px);
      border-radius: 2rem;
      border: 1px solid rgba(0, 212, 255, 0.2);
      box-shadow: 0 20px 35px -12px rgba(0,0,0,0.5);
      transition: transform 0.25s ease, border-color 0.2s;
    }

    .glass-card:hover {
      border-color: rgba(0, 212, 255, 0.5);
      transform: translateY(-3px);
    }

    .container {
      max-width: 1300px;
      margin: 0 auto;
      padding: 2rem 1.5rem;
    }

    /* animated sliding banner refined */
    .slider-banner {
      position: relative;
      width: 100%;
      height: 130px;
      overflow: hidden;
      border-radius: 2rem;
      margin: 1rem 0 2rem;
      box-shadow: 0 8px 20px rgba(0,0,0,0.4);
    }
    .slide-track {
      display: flex;
      width: calc(300%);
      animation: scrollSlides 24s infinite linear;
    }
    .slide {
      flex: 0 0 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 2rem;
      background: linear-gradient(135deg, #071126, #0f1f3a);
      font-weight: 600;
      font-size: 1.3rem;
      letter-spacing: 1px;
    }
    @keyframes scrollSlides {
      0% { transform: translateX(0);}
      20% { transform: translateX(0);}
      25% { transform: translateX(-100%);}
      45% { transform: translateX(-100%);}
      50% { transform: translateX(-200%);}
      70% { transform: translateX(-200%);}
      75% { transform: translateX(-300%);}
      95% { transform: translateX(-300%);}
      100% { transform: translateX(-400%);}
    }
    .slide i { font-size: 2rem; color: #00d4ff;}

    h1, h2, h3 {
      font-weight: 700;
      letter-spacing: -0.02em;
    }
    .gradient-text {
      background: linear-gradient(120deg, #c0e0ff, #00d4ff, #a97cff);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
    }
    .badge-group {
      display: flex;
      flex-wrap: wrap;
      gap: 0.7rem;
      margin: 1rem 0;
      justify-content: center;
    }
    .badge {
      background: rgba(0, 212, 255, 0.12);
      padding: 0.4rem 1rem;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      backdrop-filter: blur(4px);
      border: 1px solid rgba(0,212,255,0.3);
    }

    .skill-tag {
      background: #0f1a2f;
      padding: 0.3rem 0.9rem;
      border-radius: 20px;
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.8rem;
      font-weight: 500;
      color: #bbd9ff;
    }

    .grid-2col {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.8rem;
    }

    .code-block {
      background: #03070fcc;
      border-radius: 1rem;
      padding: 1rem;
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.75rem;
      border-left: 4px solid #00d4ff;
      overflow-x: auto;
      white-space: pre-wrap;
      word-break: break-word;
    }

    .pub-metrics {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 1rem;
      background: rgba(0,0,0,0.4);
      border-radius: 1.2rem;
      padding: 1rem;
    }

    footer {
      text-align: center;
      padding: 2rem 1rem 1rem;
      font-size: 0.8rem;
      border-top: 1px solid rgba(0,212,255,0.2);
      margin-top: 2rem;
    }

    a {
      color: #7cc9ff;
      text-decoration: none;
      transition: 0.2s;
    }
    a:hover {
      color: white;
      text-shadow: 0 0 5px #00d4ff;
    }

    @media (max-width: 700px) {
      .container { padding: 1rem; }
      .slide { font-size: 0.9rem; gap: 1rem; }
    }
  </style>
</head>
<body>
<div class="bg-orb"></div>

<div class="container">
  
  <!-- Header Section -->
  <div style="text-align: center; margin-bottom: 1.5rem;">
    <div style="display: inline-block; background: linear-gradient(145deg, #0a0f2a, #030617); padding: 0.6rem 1.8rem; border-radius: 60px; margin-bottom: 1rem;">
      <span style="font-weight: 600;">⚡ SAHIL MAURYA | RESEARCH SCHOLAR @ IIT MANDI</span>
    </div>
    <h1 style="font-size: 3.5rem; font-weight: 800; margin: 0.3rem 0;"><span class="gradient-text">Sahil Maurya</span></h1>
    <p style="font-size: 1.2rem; max-width: 700px; margin: 0.5rem auto;">🔐 Post-Quantum Cryptography Hardware | RISC-V SoC Architect | VLSI Researcher</p>
    <div class="badge-group">
      <span class="badge"><i class="fas fa-microchip"></i> IIT Mandi</span>
      <span class="badge"><i class="fas fa-trophy"></i> Gold Medalist M.Tech</span>
      <span class="badge"><i class="fas fa-chart-line"></i> CGPA 9.11/10</span>
      <span class="badge"><i class="fas fa-shield-alt"></i> PQC Hardware Expert</span>
    </div>
  </div>

  <!-- Animated banner (sliding topics) -->
  <div class="slider-banner">
    <div class="slide-track">
      <div class="slide"><i class="fas fa-lock"></i> POST-QUANTUM CRYPTOGRAPHY <i class="fas fa-bolt"></i></div>
      <div class="slide"><i class="fas fa-microchip"></i> RISC-V SoC ARCHITECTURE <i class="fas fa-cogs"></i></div>
      <div class="slide"><i class="fas fa-chart-simple"></i> DIGITAL VLSI DESIGN <i class="fas fa-waveform"></i></div>
      <div class="slide"><i class="fas fa-shield-hog"></i> HARDWARE SECURITY <i class="fas fa-key"></i></div>
      <div class="slide"><i class="fas fa-microchip"></i> FPGA & ASIC IMPLEMENTATION <i class="fas fa-industry"></i></div>
    </div>
  </div>

  <!-- About / Intro glass panel -->
  <div class="glass-card" style="padding: 1.8rem; margin-bottom: 2rem;">
    <div style="display: flex; flex-wrap: wrap; gap: 1rem; justify-content: space-between; align-items: center;">
      <div style="flex:2">
        <h2><i class="fas fa-user-astronaut"></i> 🔬 About Me — Architecting Secure Silicon</h2>
        <p style="margin-top: 0.8rem;">🎓 Research Scholar @ IIT Mandi (SCEE) — Building Post-Quantum Cryptographic Hardware for NIST Standards (Kyber/Dilithium). <br>
        ⚙️ Designing Secure RISC-V SoCs with custom ISA extensions. <br>
        🖥️ RTL-to-GDSII flow | PPA optimization | Side-channel resistant architectures.<br>
        🏆 Gold Medalist — M.Tech VLSI, IIIT Guwahati (CGPA 9.11/10) <br>
        📚 Publications: IEEE HiPC 2025 | IEEE SILCON 2024 | 💡 Patent filed: Approximate Modular Multiplier for R-LWE.</p>
      </div>
      <div style="flex:1; text-align: center;">
        <i class="fas fa-quote-right" style="font-size: 3rem; opacity: 0.6;"></i>
        <p style="font-style: italic; font-size: 0.9rem;">"Building hardware foundation for a post-quantum secure world — one transistor at a time."</p>
      </div>
    </div>
  </div>

  <!-- Academic Pedigree Table -->
  <div class="glass-card" style="padding: 1.6rem; margin-bottom: 2rem;">
    <h2><i class="fas fa-graduation-cap"></i> 🏛️ Academic Pedigree</h2>
    <div style="overflow-x: auto;">
      <table style="width:100%; margin-top: 1rem; border-collapse: collapse; text-align: center;">
        <thead style="background: rgba(0,212,255,0.15);">
          <tr><th>Degree</th><th>Institution</th><th>Duration</th><th>Performance</th></tr>
        </thead>
        <tbody>
          <tr><td>Ph.D. Research Scholar</td><td>IIT Mandi</td><td>2025 – Present</td><td>CGPA 8.33/10.0</td></tr>
          <tr><td>M.Tech (VLSI & Embedded)</td><td>IIIT Guwahati</td><td>2021 – 2023</td><td>CGPA 9.11/10.0 🏅 Gold Medalist</td></tr>
          <tr><td>B.Tech (Electronics & Comm)</td><td>University of Lucknow</td><td>2017 – 2021</td><td>66.1%</td></tr>
        </tbody>
      </table>
    </div>
  </div>

  <!-- Tech Stack / Skills -->
  <div class="grid-2col" style="margin-bottom: 2rem;">
    <div class="glass-card" style="padding: 1.6rem;">
      <h3><i class="fas fa-code"></i> 🔧 Hardware Languages</h3>
      <div style="margin-top: 1rem;">
        <span class="skill-tag">Verilog (Expert 5+ yrs)</span>
        <span class="skill-tag">SystemVerilog (Advanced)</span>
        <span class="skill-tag">VHDL (Intermediate)</span>
        <span class="skill-tag">C/C++ / Embedded</span>
        <span class="skill-tag">Python (Expert)</span>
        <span class="skill-tag">RISC-V Assembly</span>
      </div>
      <h3 style="margin-top: 1rem;"><i class="fas fa-tools"></i> EDA & FPGA</h3>
      <div><span class="skill-tag">Xilinx Vivado</span> <span class="skill-tag">Cadence Genus/Innovus</span> <span class="skill-tag">OpenLane/OpenROAD</span> <span class="skill-tag">ModelSim/QuestaSim</span></div>
      <h3 style="margin-top: 1rem;"><i class="fas fa-shield-hog"></i> Hardware Security</h3>
      <div><span class="skill-tag">CRYSTALS-Kyber/Dilithium</span> <span class="skill-tag">NTT Accelerators</span> <span class="skill-tag">Side-Channel Analysis</span> <span class="skill-tag">PUF/TRNG</span></div>
    </div>
    <div class="glass-card" style="padding: 1.6rem;">
      <h3><i class="fas fa-chart-simple"></i> 📊 Research Metrics & Key Achievements</h3>
      <div class="pub-metrics" style="margin-top: 1rem;">
        <div><i class="fas fa-microchip"></i> <strong>Approx Modular Multiplier</strong><br>Area -34% | Power -33% | Accuracy >99%</div>
        <div><i class="fas fa-brain"></i> <strong>Neuromorphic RISC-V</strong><br>Energy savings 40% avg (HiPC 2025)</div>
        <div><i class="fas fa-lock"></i> <strong>Kyber NTT Engine</strong><br>245 MHz | 1.28 Gbps | 2.8k LUTs</div>
      </div>
      <h3 style="margin-top: 1rem;"><i class="fas fa-award"></i> Certifications</h3>
      <div><span class="skill-tag">VSD STA</span><span class="skill-tag">Cadence RTL to GDS</span><span class="skill-tag">VLSI Design with Vivado</span><span class="skill-tag">Python for Data Science</span></div>
      <div style="margin-top: 1rem;"><i class="fas fa-file-alt"></i> <strong>Patent filed</strong> — Approximate Modular Multiplier for R-LWE Cryptosystems</div>
    </div>
  </div>

  <!-- Flagship Projects -->
  <h2 style="margin: 0.5rem 0 1rem;"><i class="fas fa-microchip"></i> 💻 Flagship Research Projects</h2>
  <div class="grid-2col" style="margin-bottom: 2rem;">
    <div class="glass-card" style="padding: 1.5rem;">
      <h3>🔐 CRYSTALS-Kyber NTT Hardware Accelerator</h3>
      <div class="code-block">
        // 4-parallel pipelined NTT with banked memory<br>
        // 245 MHz, 1.28 Gbps, 2845 LUTs, 8 DSPs<br>
        module ntt_processing_element #(N=256, Q=3329)(...);<br>
        &nbsp;&nbsp; // butterfly + Barrett reduction → high throughput<br>
        endmodule
      </div>
      <p><strong>🏆 Results:</strong> KeyGen 12.4μs | Encaps 14.1μs | Decaps 15.2μs — 41% ATP improvement over baseline.</p>
    </div>
    <div class="glass-card" style="padding: 1.5rem;">
      <h3>🧠 Neuromorphic Adaptive Precision RISC-V (HiPC 2025)</h3>
      <div class="code-block">
        // Dynamic precision scaling 8-bit to 32-bit based on neuronal spikes<br>
        // Adaptive voltage/freq scaling — energy reduction up to 52% for SNNs<br>
        // Real-time precision management unit integrated with ALU
      </div>
      <p><strong>📈 Gains:</strong> Image recognition +45% energy saving, Spiking Neural Nets 52% lower power.</p>
    </div>
    <div class="glass-card" style="padding: 1.5rem;">
      <h3>📊 Approximate Modular Multiplier (IEEE SILCON 2024)</h3>
      <div class="code-block">
        module kyber_approx_modular_multiplier #(Q=3329) (<br>
        &nbsp;&nbsp; input [16:0] a,b, output [16:0] result<br>
        ); // 34% area reduction, 33% power saving, <1% error
      </div>
      <p>Patent filed — first approximation technique for R-LWE with error compensation logic, enabling lightweight PQC on edge devices.</p>
    </div>
    <div class="glass-card" style="padding: 1.5rem;">
      <h3>🏗️ RISC-V SoC + PQC Coprocessor</h3>
      <div class="code-block">
        AXI/APB interconnect with Kyber accelerator (APB slave)<br>
        • Control registers, NTT engine, TRNG, PUF-based key storage<br>
        • Custom PQC instructions decoder in RISC-V pipeline
      </div>
      <p>🔒 Privilege separation & memory-mapped accelerator for Kyber ops — side-channel resistant layout.</p>
    </div>
  </div>

  <!-- PQC+RISC-V SoC Integration Architecture (ASCII enhanced) -->
  <div class="glass-card" style="padding: 1.8rem; margin-bottom: 2rem;">
    <h2><i class="fas fa-sitemap"></i> 🏗️ PQC + RISC-V SoC Integration Architecture</h2>
    <div class="code-block" style="background: #00000055; font-size: 0.7rem;">
      ╔═══════════════════════════════════════════════════════════════╗<br>
      ║     RISC-V Core (RV32IM) + PQC Custom Extensions              ║<br>
      ║  ┌────────────┐ ┌───────────┐ ┌─────────────────────────┐   ║<br>
      ║  │Reg File    │ │ ALU (Mul) │ │ Ctrl: PQC Instr decode  │   ║<br>
      ║  └────────────┘ └───────────┘ └───────────┬─────────────┘   ║<br>
      ║               AXI/APB interconnect          │                 ║<br>
      ║      ┌──────────────────────────────────────▼─────────────┐  ║<br>
      ║      │   Kyber Hardware Accelerator (APB slave)          │  ║<br>
      ║      │  • NTT Engine • Modular Mult • Sampler • TRNG     │  ║<br>
      ║      │  • Side-channel shield • Masked implementation    │  ║<br>
      ║      └───────────────────────────────────────────────────┘  ║<br>
      ║   🔐 Memory map: 0x4000_0000 control | 0x4000_1000 poly buf ║<br>
      ╚═══════════════════════════════════════════════════════════════╝
    </div>
    <p style="margin-top: 0.8rem;"><i class="fas fa-check-circle" style="color:#00d4ff"></i> Secure key storage (PUF) & side-channel resistant NTT — quantum-safe root of trust.</p>
  </div>

  <!-- Publications & research metrics interactive -->
  <div class="glass-card" style="padding: 1.6rem; margin-bottom: 2rem;">
    <h2><i class="fas fa-newspaper"></i> 📚 Publications & Impact</h2>
    <div style="display: flex; flex-wrap: wrap; gap: 1.5rem; justify-content: space-between;">
      <div style="flex:1;">
        <ul style="list-style-type: none;">
          <li>✔ <strong>Neuromorphic Adaptive Precision RISC-V</strong> — IEEE HiPC 2025 (Accepted)</li>
          <li>✔ <strong>Approximate Modular Multipliers for R-LWE</strong> — IEEE SILCON 2024 (Best Paper Nominee)</li>
        </ul>
        <div class="badge-group" style="margin-top: 1rem;">
          <span><i class="fas fa-chart-line"></i> 2 conference papers</span>
          <span><i class="fas fa-file-powerpoint"></i> Patent filed</span>
          <span><i class="fas fa-citation"></i> 12+ citations (growing)</span>
        </div>
      </div>
      <div style="flex:1; background: rgba(0,0,0,0.3); border-radius: 1rem; padding: 0.8rem;">
        <p><i class="fas fa-chart-pie"></i> <strong>Kyber NTT Accelerator Metrics</strong><br>🔹 Frequency: 245 MHz &nbsp;| 🔹 Throughput: 1.28 Gbps<br>🔹 LUTs: 2845 &nbsp;| 🔹 KeyGen: 12.4μs</p>
        <p><i class="fas fa-microchip"></i> <strong>Area-Power Optimization (approx mult)</strong><br>📉 Area: -34% &nbsp;⚡ Power: -33% &nbsp;🎯 Accuracy: 99.2%</p>
      </div>
    </div>
  </div>

  <!-- Current research directions table -->
  <div class="glass-card" style="padding: 1.6rem;">
    <h2><i class="fas fa-flask"></i> 🔬 Current Research Directions</h2>
    <div style="overflow-x: auto;">
      <table style="width:100%; margin-top: 0.8rem; border-collapse: collapse;">
        <thead><tr style="border-bottom:1px solid #00d4ff40;"><th>Direction</th><th>Algorithm</th><th>Focus</th><th>Target</th></tr></thead>
        <tbody>
          <tr><td>High-Throughput NTT</td><td>Kyber</td><td>8-parallel pipelined</td><td>IEEE TCAS-I</td></tr>
          <tr><td>Masked PQC</td><td>Kyber/Dilithium</td><td>Side-channel resistance</td><td>CHES 2026</td></tr>
          <tr><td>RISC-V PQC Extensions</td><td>Kyber</td><td>Custom ISA</td><td>VLSID 2026</td></tr>
          <tr><td>PUF-based Key Storage</td><td>Kyber</td><td>Hardware root of trust</td><td>HOST 2026</td></tr>
        </tbody>
      </table>
    </div>
  </div>

  <!-- GitHub stats & connect -->
  <div class="grid-2col" style="margin: 2rem 0;">
    <div class="glass-card" style="padding: 1.5rem; text-align: center;">
      <i class="fab fa-github" style="font-size: 2rem;"></i>
      <h3>GitHub Activity</h3>
      <img src="https://github-readme-stats.vercel.app/api?username=sahilmaurya007&show_icons=true&theme=dark&hide_border=true&bg_color=00000000&title_color=00d4ff&icon_color=aa7eff" width="100%" style="border-radius: 1rem;">
    </div>
    <div class="glass-card" style="padding: 1.5rem;">
      <h3><i class="fas fa-envelope"></i> 📫 Connect & Collaborate</h3>
      <p><i class="fas fa-inbox"></i> <strong>Email:</strong> <a href="mailto:d24204@students.iitmandi.ac.in">d24204@students.iitmandi.ac.in</a><br>
      <i class="fab fa-linkedin"></i> <a href="#">linkedin.com/in/sahilmaurya007</a><br>
      <i class="fas fa-map-marker-alt"></i> IIT Mandi, Kamand, HP | Permanent: Lucknow, UP<br>
      <i class="fas fa-phone-alt"></i> +91-7270020537</p>
      <div class="badge-group">
        <a href="#"><span class="badge"><i class="fab fa-google"></i> Google Scholar</span></a>
        <a href="#"><span class="badge"><i class="fab fa-researchgate"></i> ResearchGate</span></a>
      </div>
      <p style="margin-top: 1rem;"><i class="fas fa-quote-left"></i> "Building quantum-resistant silicon for a post-quantum world — every transistor counts."</p>
    </div>
  </div>

  <footer>
    <p>© 2025 Sahil Maurya | IIT Mandi Research Scholar | Hardware Security & Post-Quantum Cryptography</p>
    <p style="font-size: 0.7rem;">Last Updated: March 2026 | Dynamic background & futuristic design</p>
  </footer>
</div>
</body>
</html>
