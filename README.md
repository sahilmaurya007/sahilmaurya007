<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sahil Maurya | Research Scholar @ IIT Mandi | VLSI | PQC | RISC-V</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Fira Code', 'Share Tech Mono', 'Courier New', monospace;
            background: linear-gradient(135deg, #0a0f1a 0%, #0a1a2a 25%, #0a0f2a 50%, #0a1a2a 75%, #0a0f1a 100%);
            color: #e0e0e0;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Animated Circuit Board Background */
        .circuit-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -2;
            background: radial-gradient(circle at 20% 30%, rgba(0, 40, 60, 0.4) 0%, rgba(0, 0, 0, 0.85) 100%);
        }

        .circuit-bg::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(rgba(0, 212, 255, 0.05) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 212, 255, 0.05) 1px, transparent 1px);
            background-size: 40px 40px;
            animation: drift 30s linear infinite;
        }

        .circuit-bg::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><path fill="none" stroke="rgba(0,212,255,0.1)" stroke-width="0.5" d="M10,10 L30,10 L30,30 L10,30 Z M50,20 L70,20 L70,40 L50,40 Z M80,60 L95,60 L95,75 L80,75 Z M20,70 L40,70 L40,90 L20,90 Z M60,80 L75,80 L75,95 L60,95 Z"/></svg>');
            background-repeat: repeat;
            background-size: 80px;
            opacity: 0.3;
            animation: rotate 60s linear infinite;
        }

        @keyframes drift {
            0% { transform: translateY(0); }
            100% { transform: translateY(50px); }
        }

        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        /* Floating Particles - Chip Dust Effect */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            pointer-events: none;
        }

        .particle {
            position: absolute;
            background: radial-gradient(circle, rgba(0, 212, 255, 0.8), rgba(124, 58, 237, 0.4));
            border-radius: 50%;
            animation: float linear infinite;
            box-shadow: 0 0 5px rgba(0,212,255,0.5);
        }

        @keyframes float {
            0% { transform: translateY(100vh) translateX(0) rotate(0deg); opacity: 0; }
            10% { opacity: 0.8; }
            90% { opacity: 0.8; }
            100% { transform: translateY(-10vh) translateX(50px) rotate(360deg); opacity: 0; }
        }

        /* Main Container */
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 1;
        }

        /* Glassmorphism Effect */
        .glass {
            background: rgba(10, 20, 30, 0.6);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(0, 212, 255, 0.25);
            border-radius: 20px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
        }

        /* Header Section with Chip Design */
        .header {
            text-align: center;
            padding: 50px 20px 40px;
            background: linear-gradient(135deg, rgba(0, 0, 0, 0.75), rgba(0, 40, 60, 0.6));
            border-radius: 30px;
            margin-bottom: 40px;
            backdrop-filter: blur(12px);
            border: 1px solid rgba(0, 212, 255, 0.4);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.5), inset 0 1px 0 rgba(255,255,255,0.1);
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(0,212,255,0.05), transparent);
            transform: rotate(45deg);
            animation: shimmer 8s infinite;
        }

        @keyframes shimmer {
            0% { transform: translateX(-100%) rotate(45deg); }
            100% { transform: translateX(100%) rotate(45deg); }
        }

        .header h1 {
            font-size: 4.2rem;
            background: linear-gradient(135deg, #00d4ff, #7c3aed, #00ffaa, #00d4ff);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 15px;
            letter-spacing: 3px;
            animation: gradientShift 4s ease infinite;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .header .subtitle {
            font-size: 1.2rem;
            color: #00d4ff;
            letter-spacing: 2px;
            margin-bottom: 10px;
        }

        .header .affiliation {
            font-size: 1rem;
            color: #8b949e;
        }

        /* Typing Animation */
        .typing-container {
            margin: 20px 0;
            font-family: 'Fira Code', monospace;
            font-size: 1.1rem;
        }

        .typed-text {
            color: #00d4ff;
            border-right: 2px solid #00d4ff;
            animation: blink 0.7s infinite;
        }

        @keyframes blink {
            0%, 100% { border-color: transparent; }
            50% { border-color: #00d4ff; }
        }

        /* Navigation */
        .nav {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .nav a {
            color: #e0e0e0;
            text-decoration: none;
            padding: 10px 20px;
            background: rgba(0, 212, 255, 0.1);
            border-radius: 30px;
            transition: all 0.3s ease;
            border: 1px solid rgba(0, 212, 255, 0.3);
            font-weight: 500;
        }

        .nav a:hover {
            background: rgba(0, 212, 255, 0.3);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 212, 255, 0.2);
        }

        /* Badges */
        .badge-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 12px;
            margin: 25px 0;
        }

        .badge {
            padding: 8px 16px;
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.15), rgba(124, 58, 237, 0.15));
            border-radius: 20px;
            font-size: 0.85rem;
            border: 1px solid rgba(0, 212, 255, 0.3);
            transition: transform 0.2s;
        }

        .badge:hover {
            transform: scale(1.05);
            border-color: #00d4ff;
        }

        /* Section Styles */
        .section {
            margin-bottom: 50px;
        }

        .section-title {
            font-size: 2rem;
            margin-bottom: 25px;
            padding-bottom: 10px;
            border-bottom: 2px solid #00d4ff;
            display: inline-block;
            background: linear-gradient(135deg, #00d4ff, #7c3aed);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        /* Card Grid */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 25px;
            margin-top: 20px;
        }

        .card {
            background: rgba(15, 25, 35, 0.7);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 25px;
            border: 1px solid rgba(0, 212, 255, 0.2);
            transition: all 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: rgba(0, 212, 255, 0.5);
            box-shadow: 0 10px 30px rgba(0, 212, 255, 0.1);
        }

        .card h3 {
            color: #00d4ff;
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        /* Table Styles */
        .research-table {
            width: 100%;
            border-collapse: collapse;
            background: rgba(10, 20, 30, 0.6);
            border-radius: 15px;
            overflow: hidden;
        }

        .research-table th, .research-table td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid rgba(0, 212, 255, 0.2);
        }

        .research-table th {
            background: rgba(0, 212, 255, 0.15);
            color: #00d4ff;
            font-weight: 600;
        }

        .research-table tr:hover {
            background: rgba(0, 212, 255, 0.05);
        }

        /* Progress Bar */
        .progress-bar {
            width: 100%;
            height: 8px;
            background: rgba(255,255,255,0.1);
            border-radius: 4px;
            overflow: hidden;
            margin-top: 8px;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, #00d4ff, #7c3aed);
            border-radius: 4px;
            transition: width 1s ease;
        }

        /* Code Block */
        .code-block {
            background: #0a0f1a;
            border-radius: 12px;
            padding: 20px;
            margin: 20px 0;
            overflow-x: auto;
            border: 1px solid rgba(0, 212, 255, 0.3);
            font-family: 'Fira Code', monospace;
            font-size: 0.85rem;
        }

        /* Architecture Diagram */
        .arch-diagram {
            background: rgba(0, 0, 0, 0.4);
            border-radius: 15px;
            padding: 20px;
            font-family: monospace;
            white-space: pre;
            overflow-x: auto;
            font-size: 0.7rem;
            line-height: 1.4;
        }

        /* Footer */
        .footer {
            text-align: center;
            padding: 40px 20px;
            margin-top: 50px;
            background: linear-gradient(135deg, rgba(0,0,0,0.8), rgba(0,40,60,0.6));
            border-radius: 30px;
            border: 1px solid rgba(0, 212, 255, 0.2);
        }

        /* Stats Grid */
        .stats-grid {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .stat-card {
            background: rgba(0, 212, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            min-width: 150px;
            border: 1px solid rgba(0, 212, 255, 0.3);
        }

        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #00d4ff;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .header h1 { font-size: 2.5rem; }
            .section-title { font-size: 1.5rem; }
            .card-grid { grid-template-columns: 1fr; }
            .arch-diagram { font-size: 0.5rem; }
        }
    </style>
</head>
<body>
    <div class="circuit-bg"></div>
    <div class="particles" id="particles"></div>

    <div class="container">
        <!-- Header Section -->
        <div class="header">
            <h1>SAHIL MAURYA</h1>
            <div class="subtitle">🔬 Research Scholar | Digital VLSI | Post-Quantum Cryptography | RISC-V SoC Architect</div>
            <div class="affiliation">🏛️ Indian Institute of Technology (IIT) Mandi | SCEE Department</div>
            
            <div class="typing-container">
                <span id="typed-text" class="typed-text"></span><span class="cursor">|</span>
            </div>

            <div class="badge-container">
                <span class="badge">🏅 Gold Medalist M.Tech VLSI</span>
                <span class="badge">🔐 PQC Hardware Accelerators</span>
                <span class="badge">⚡ RISC-V SoC Design</span>
                <span class="badge">🖥️ FPGA/ASIC Expert</span>
                <span class="badge">📊 CGPA 9.11/10.0</span>
            </div>
        </div>

        <!-- Navigation -->
        <div class="nav">
            <a href="#about">📌 About Me</a>
            <a href="#education">🎓 Education</a>
            <a href="#skills">🛠️ Skills</a>
            <a href="#projects">💻 Projects</a>
            <a href="#publications">📚 Publications</a>
            <a href="#contact">📫 Contact</a>
        </div>

        <!-- About Section -->
        <div class="section" id="about">
            <h2 class="section-title">🔬 About Me</h2>
            <div class="card">
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    I am a <strong>Research Scholar at IIT Mandi (SCEE Department)</strong> specializing in <strong>Digital VLSI Design</strong>, 
                    <strong>Post-Quantum Cryptography (PQC) Hardware Acceleration</strong>, and <strong>Secure RISC-V SoC Architectures</strong>.
                    My research focuses on developing quantum-resistant cryptographic accelerators for NIST-standardized algorithms 
                    (CRYSTALS-Kyber, Dilithium) with optimized Power, Performance, and Area (PPA).
                </p>
                <br>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    With a <strong>Gold Medalist M.Tech in VLSI</strong> from IIIT Guwahati (CGPA: 9.11/10.0), I have published research at top-tier 
                    venues including <strong>IEEE HiPC 2025</strong> and <strong>IEEE SILCON 2024</strong>. My goal is to build the hardware 
                    foundation for a post-quantum secure world — one transistor, one instruction, one algorithm at a time.
                </p>
            </div>
        </div>

        <!-- Education Section -->
        <div class="section" id="education">
            <h2 class="section-title">🎓 Academic Pedigree</h2>
            <table class="research-table">
                <thead>
                    <tr><th>Degree</th><th>Institution</th><th>Year</th><th>Performance</th></tr>
                </thead>
                <tbody>
                    <tr><td><b>Ph.D. Research Scholar</b></td><td>IIT Mandi</td><td>2025 - Present</td><td>CGPA: 8.33/10.0</td></tr>
                    <tr><td><b>M.Tech (VLSI & Embedded)</b></td><td>IIIT Guwahati</td><td>2021 - 2023</td><td>CGPA: 9.11/10.0 🏅 Gold Medalist</td></tr>
                    <tr><td><b>B.Tech (Electronics & Comm)</b></td><td>University of Lucknow</td><td>2017 - 2021</td><td>66.1%</td></tr>
                    <tr><td><b>Higher Secondary</b></td><td>UP Board</td><td>2016</td><td>85%</td></tr>
                </tbody>
            </table>
        </div>

        <!-- Skills Section -->
        <div class="section" id="skills">
            <h2 class="section-title">🛠️ Technical Arsenal</h2>
            <div class="card-grid">
                <div class="card">
                    <h3>🔧 Hardware Description</h3>
                    <div>Verilog <div class="progress-bar"><div class="progress-fill" style="width: 95%"></div></div></div>
                    <div>SystemVerilog <div class="progress-bar"><div class="progress-fill" style="width: 85%"></div></div></div>
                    <div>VHDL <div class="progress-bar"><div class="progress-fill" style="width: 70%"></div></div></div>
                    <div>Chisel <div class="progress-bar"><div class="progress-fill" style="width: 50%"></div></div></div>
                </div>
                <div class="card">
                    <h3>📀 EDA Tools</h3>
                    <div>Xilinx Vivado (Expert)</div>
                    <div>Cadence Genus/Innovus (Advanced)</div>
                    <div>OpenLane/OpenROAD (Advanced)</div>
                    <div>ModelSim/Questasim (Expert)</div>
                </div>
                <div class="card">
                    <h3>🔐 Security Domains</h3>
                    <div>Post-Quantum Cryptography (Kyber/Dilithium)</div>
                    <div>Side-Channel Analysis & Countermeasures</div>
                    <div>RISC-V Security Extensions</div>
                    <div>PUF/TRNG Design</div>
                </div>
                <div class="card">
                    <h3>💻 Programming</h3>
                    <div>Python (Expert) <div class="progress-bar"><div class="progress-fill" style="width: 90%"></div></div></div>
                    <div>C/C++ (Advanced) <div class="progress-bar"><div class="progress-fill" style="width: 85%"></div></div></div>
                    <div>RISC-V Assembly (Advanced) <div class="progress-bar"><div class="progress-fill" style="width: 80%"></div></div></div>
                    <div>TCL/Python Scripting (Advanced)</div>
                </div>
            </div>
        </div>

        <!-- Research Projects Section -->
        <div class="section" id="projects">
            <h2 class="section-title">💻 Research Projects</h2>
            
            <!-- Project 1: Kyber NTT Accelerator -->
            <div class="card" style="margin-bottom: 25px;">
                <h3>🔐 CRYSTALS-Kyber NTT Hardware Accelerator</h3>
                <p><strong>Problem:</strong> CRYSTALS-Kyber requires high-performance NTT operations that are computationally intensive on general-purpose processors.</p>
                <p><strong>Solution:</strong> 4-parallel NTT architecture with banked memory and pipelined Barrett reduction.</p>
                <div class="arch-diagram">
                    <pre>
┌─────────────────────────────────────────────────────────────────┐
│                    NTT CORE ARCHITECTURE                        │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐         │
│  │   PE 0      │    │   PE 1      │    │   PE 2      │    PE 3 │
│  │ Butterfly   │    │ Butterfly   │    │ Butterfly   │ Butterfly│
│  │ + Barrett   │    │ + Barrett   │    │ + Barrett   │ + Barrett│
│  └─────────────┘    └─────────────┘    └─────────────┘         │
│         │                │                │                     │
│         └────────────────┼────────────────┘                     │
│                          ▼                                      │
│              ┌─────────────────────┐                           │
│              │   Banked Memory     │                           │
│              │  (4 Banks x 64)     │                           │
│              └─────────────────────┘                           │
└─────────────────────────────────────────────────────────────────┘
                    </pre>
                </div>
                <p><strong>Results:</strong> 245 MHz | 1.28 Gbps | 2,845 LUTs | 12.4 μs Key Generation</p>
            </div>

            <!-- Project 2: Approximate Modular Multiplier -->
            <div class="card" style="margin-bottom: 25px;">
                <h3>📊 Approximate Modular Multiplier for R-LWE Cryptosystems</h3>
                <p><strong>Published in IEEE SILCON 2024</strong></p>
                <p><strong>Innovation:</strong> 34% area reduction, 33% power savings with &lt;1% accuracy loss for Kyber.</p>
                <div class="code-block">
                    <pre style="margin:0; color:#00d4ff;">
// Approximate Modular Multiplier for CRYSTALS-Kyber
module approx_modular_multiplier #(parameter Q = 3329)(
    input  logic [16:0] a, b,
    output logic [16:0] result
);
    // Adaptive approximation with error compensation
    // 34% area reduction | 33% power savings
endmodule
                    </pre>
                </div>
            </div>

            <!-- Project 3: Neuromorphic RISC-V Processor -->
            <div class="card">
                <h3>🧠 Neuromorphic Adaptive Precision RISC-V Processor</h3>
                <p><strong>Accepted at IEEE HiPC 2025</strong></p>
                <p><strong>Innovation:</strong> First RISC-V processor with real-time precision scaling for neuromorphic computing.</p>
                <p><strong>Results:</strong> 45% energy reduction for image recognition | 52% for spiking neural networks</p>
            </div>
        </div>

        <!-- Publications Section -->
        <div class="section" id="publications">
            <h2 class="section-title">📚 Publications & Research Impact</h2>
            <table class="research-table">
                <thead>
                    <tr><th>Title</th><th>Venue</th><th>Year</th><th>Status</th></tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Neuromorphic Adaptive Precision RISC-V Processor with Real-Time Precision Scaling and Neuronal State Management</td>
                        <td>IEEE HiPC</td>
                        <td>2025</td>
                        <td>✅ Accepted</td>
                    </tr>
                    <tr>
                        <td>Approximate Modular Multipliers for R-LWE Cryptosystems on FPGAs and ASICs</td>
                        <td>IEEE SILCON</td>
                        <td>2024</td>
                        <td>✅ Published</td>
                    </tr>
                </tbody>
            </table>

            <div class="stats-grid">
                <div class="stat-card"><div class="stat-number">34%</div><div>Area Reduction</div></div>
                <div class="stat-card"><div class="stat-number">33%</div><div>Power Savings</div></div>
                <div class="stat-card"><div class="stat-number">245MHz</div><div>Max Frequency</div></div>
                <div class="stat-card"><div class="stat-number">1.28Gbps</div><div>Throughput</div></div>
            </div>
        </div>

        <!-- PQC + RISC-V Integration Architecture -->
        <div class="section">
            <h2 class="section-title">🏗️ PQC + RISC-V SoC Architecture</h2>
            <div class="card">
                <div class="arch-diagram">
                    <pre>
╔═══════════════════════════════════════════════════════════════════════════════╗
║                         RISC-V SoC with PQC Coprocessor                        ║
╠═══════════════════════════════════════════════════════════════════════════════╣
║                                                                               ║
║   ┌─────────────────────────────────────────────────────────────────────┐     ║
║   │                    RISC-V Core (RV32IM)                             │     ║
║   │  ┌──────────────┐  ┌──────────────┐  ┌──────────────────────────┐ │     ║
║   │  │ Register File│  │     ALU      │  │    Control Unit          │ │     ║
║   │  │ (32 x 32-bit)│  │  ADD/SUB/MUL │  │  • PQC Instruction Decode│ │     ║
║   │  └──────────────┘  └──────────────┘  └──────────────────────────┘ │     ║
║   └─────────────────────────────────────────────────────────────────────┘     ║
║                                    │                                          ║
║                                    ▼                                          ║
║                        ┌─────────────────────┐                               ║
║                        │   AXI / APB Bus     │                               ║
║                        │    Interconnect     │                               ║
║                        └──────────┬──────────┘                               ║
║                                   │                                          ║
║         ┌─────────────────────────┼─────────────────────────┐               ║
║         │                         │                         │               ║
║         ▼                         ▼                         ▼               ║
║   ┌─────────────┐          ┌─────────────┐          ┌─────────────┐        ║
║   │ APB Bridge  │          │ DDR3/BRAM   │          │   UART/GPIO │        ║
║   │   & Decoder │          │ Controller  │          │  Interface  │        ║
║   └──────┬──────┘          └─────────────┘          └─────────────┘        ║
║          │                                                                   ║
║          ▼                                                                   ║
║   ┌─────────────────────────────────────────────────────────────────────┐   ║
║   │              Kyber Hardware Accelerator (APB Slave)                 │   ║
║   │  ┌───────────────────────────────────────────────────────────────┐ │   ║
║   │  │ Control Reg │ Status Reg │ Data FIFO │ Key Storage (PUF)     │ │   ║
║   │  ├───────────────────────────────────────────────────────────────┤ │   ║
║   │  │ NTT Engine │ Modular Mult │ Sampler │ TRNG │ Side-Channel Shield│ │   ║
║   │  └───────────────────────────────────────────────────────────────┘ │   ║
║   └─────────────────────────────────────────────────────────────────────┘   ║
║                                                                               ║
║   🔐 Memory Mapping: 0x4000_0000 - Control | 0x4000_1000 - Polynomial Buffer │
╚═══════════════════════════════════════════════════════════════════════════════╝
                    </pre>
                </div>
            </div>
        </div>

        <!-- GitHub Stats -->
        <div class="section">
            <h2 class="section-title">📊 GitHub Analytics</h2>
            <div align="center">
                <img width="48%" src="https://github-readme-stats.vercel.app/api?username=sahilmaurya007&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0f1a&title_color=00d4ff&icon_color=7c3aed&text_color=e0e0e0" />
                <img width="48%" src="https://github-readme-streak-stats.herokuapp.com/?user=sahilmaurya007&theme=tokyonight&hide_border=true&background=0a0f1a&ring=00d4ff&fire=7c3aed&currStreakLabel=00d4ff" />
            </div>
            <div align="center" style="margin-top: 20px;">
                <img width="80%" src="https://github-readme-activity-graph.vercel.app/graph?username=sahilmaurya007&theme=github-compact&bg_color=0a0f1a&color=00d4ff&line=7c3aed&point=00d4ff&area=true&hide_border=true" />
            </div>
        </div>

        <!-- Contact Section -->
        <div class="footer" id="contact">
            <h2 class="section-title" style="border-bottom: none;">📫 Connect With Me</h2>
            <div class="badge-container">
                <a href="mailto:d24204@students.iitmandi.ac.in" style="text-decoration: none;"><span class="badge">📧 d24204@students.iitmandi.ac.in</span></a>
                <a href="https://github.com/sahilmaurya007" style="text-decoration: none;"><span class="badge">🐙 GitHub: sahilmaurya007</span></a>
                <a href="https://linkedin.com/in/sahilmaurya007" style="text-decoration: none;"><span class="badge">🔗 LinkedIn: sahilmaurya007</span></a>
                <span class="badge">📞 +91-7270020537</span>
            </div>
            <div style="margin-top: 30px;">
                <p>📍 <strong>Current Address:</strong> IIT Mandi, Kamand Campus, Mandi, Himachal Pradesh - 175075</p>
                <p>🏠 <strong>Permanent Address:</strong> Janki Vihar Colony, Jankipuram, Lucknow, UP - 226021</p>
            </div>
            <hr style="border-color: rgba(0,212,255,0.3); margin: 25px 0;">
            <div align="center">
                <pre style="font-family: monospace; font-size: 0.7rem; color: #00d4ff;">
╔═══════════════════════════════════════════════════════════════════════════════╗
║  🔐 Building Quantum-Resistant Silicon for a Post-Quantum World 🔐            ║
║                                                                               ║
║  "The only way to protect against quantum threats is to build security       ║
║   into the hardware from the ground up — every transistor counts."           ║
║                                                                               ║
║                              — Sahil Maurya                                   ║
╚═══════════════════════════════════════════════════════════════════════════════╝
                </pre>
            </div>
            <div style="margin-top: 20px;">
                <img src="https://komarev.com/ghpvc/?username=sahilmaurya007&color=blueviolet&style=flat-square" alt="Profile Views" />
            </div>
            <p style="margin-top: 20px; font-size: 0.8rem;">© 2025 Sahil Maurya | IIT Mandi Research Scholar | Hardware Security & Post-Quantum Cryptography</p>
        </div>
    </div>

    <script>
        // Typing Animation
        const texts = [
            "🔐 Building Quantum-Resistant Hardware Accelerators",
            "⚡ Designing Secure RISC-V SoC Pipelines",
            "🖥️ RTL to GDSII — Every Transistor Counts",
            "🔒 Synthesizing Post-Quantum Cryptographic IPs",
            "💎 Hardware Security for the Quantum Era"
        ];
        let textIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        const typedElement = document.getElementById('typed-text');

        function typeEffect() {
            const currentText = texts[textIndex];
            if (isDeleting) {
                typedElement.textContent = currentText.substring(0, charIndex - 1);
                charIndex--;
                if (charIndex === 0) {
                    isDeleting = false;
                    textIndex = (textIndex + 1) % texts.length;
                }
            } else {
                typedElement.textContent = currentText.substring(0, charIndex + 1);
                charIndex++;
                if (charIndex === currentText.length) {
                    isDeleting = true;
                    setTimeout(typeEffect, 2000);
                    return;
                }
            }
            setTimeout(typeEffect, isDeleting ? 50 : 100);
        }
        typeEffect();

        // Particle Generation
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            for (let i = 0; i < 80; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                const size = Math.random() * 4 + 1;
                particle.style.width = size + 'px';
                particle.style.height = size + 'px';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.animationDuration = Math.random() * 15 + 8 + 's';
                particle.style.animationDelay = Math.random() * 10 + 's';
                particlesContainer.appendChild(particle);
            }
        }
        createParticles();
    </script>
</body>
</html>
