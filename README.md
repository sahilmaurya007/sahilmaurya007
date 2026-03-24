```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sahil Maurya | PQC Hardware Architect | IIT Mandi</title>
    <link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono:wght@400;700&family=Orbitron:wght@400;700;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Share Tech Mono', monospace;
            background: linear-gradient(135deg, #0a0f1a 0%, #1a1f3a 25%, #0a2f4a 50%, #1a472a 75%, #0a0f2a 100%);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
            color: #e0e0e0;
            line-height: 1.6;
            overflow-x: hidden;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            text-align: center;
            padding: 60px 0;
            position: relative;
        }

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><radialGradient id="g" cx="50%" cy="50%"><stop offset="0%" stop-color="%2300d4ff" stop-opacity="0.1"/><stop offset="50%" stop-color="%237c3aed" stop-opacity="0.05"/><stop offset="100%" stop-color="%23ff4d4d" stop-opacity="0"/></radialGradient></defs><rect width="100" height="100" fill="url(%23g)"/></svg>');
            animation: pulse 4s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 0.7; transform: scale(1.05); }
        }

        .name-title {
            font-family: 'Orbitron', monospace;
            font-size: clamp(2.5rem, 6vw, 5rem);
            background: linear-gradient(45deg, #00d4ff, #7c3aed, #ff4d4d, #ffd700);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientText 3s ease infinite;
            margin-bottom: 10px;
            text-shadow: 0 0 30px rgba(0, 212, 255, 0.5);
        }

        @keyframes gradientText {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .subtitle {
            font-size: clamp(1rem, 2.5vw, 1.5rem);
            color: #00d4ff;
            font-weight: 700;
            text-shadow: 0 0 20px rgba(0, 212, 255, 0.3);
        }

        /* Sliding Banner */
        .tech-banner {
            margin: 50px 0;
            height: 200px;
            overflow: hidden;
            border-radius: 25px;
            box-shadow: 0 20px 60px rgba(0, 212, 255, 0.3);
            position: relative;
            background: linear-gradient(145deg, rgba(10,15,26,0.9), rgba(26,47,42,0.9));
            border: 2px solid rgba(0, 212, 255, 0.3);
        }

        .banner-slides {
            display: flex;
            height: 100%;
            animation: slideBanner 25s infinite linear;
        }

        .banner-slide {
            min-width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 50px;
            font-size: clamp(2rem, 4vw, 3.5rem);
            font-weight: bold;
            color: #00d4ff;
            text-shadow: 0 0 20px rgba(0, 212, 255, 0.8);
        }

        .banner-slide:nth-child(1) { background: linear-gradient(135deg, rgba(10,15,26,0.95), rgba(10,47,108,0.95)); }
        .banner-slide:nth-child(2) { background: linear-gradient(135deg, rgba(26,42,74,0.95), rgba(10,47,58,0.95)); }
        .banner-slide:nth-child(3) { background: linear-gradient(135deg, rgba(10,47,58,0.95), rgba(26,74,42,0.95)); }
        .banner-slide:nth-child(4) { background: linear-gradient(135deg, rgba(26,74,42,0.95), rgba(42,10,74,0.95)); }
        .banner-slide:nth-child(5) { background: linear-gradient(135deg, rgba(42,10,74,0.95), rgba(10,15,26,0.95)); }

        @keyframes slideBanner {
            0% { transform: translateX(0); }
            20% { transform: translateX(0); }
            25% { transform: translateX(-100%); }
            45% { transform: translateX(-100%); }
            50% { transform: translateX(-200%); }
            70% { transform: translateX(-200%); }
            75% { transform: translateX(-300%); }
            95% { transform: translateX(-300%); }
            100% { transform: translateX(-400%); }
        }

        /* Typing Animation */
        .typing-container {
            margin: 40px 0;
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .typing-text {
            font-family: 'Share Tech Mono', monospace;
            font-size: clamp(1.1rem, 2.5vw, 1.4rem);
            color: #00d4ff;
            text-shadow: 0 0 15px rgba(0, 212, 255, 0.6);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 0 0 15px rgba(0, 212, 255, 0.6); }
            to { text-shadow: 0 0 25px rgba(0, 212, 255, 0.9), 0 0 35px rgba(124, 58, 237, 0.5); }
        }

        /* Badges */
        .badges {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            margin: 40px 0;
        }

        .badge {
            padding: 12px 24px;
            background: linear-gradient(145deg, rgba(0,212,255,0.2), rgba(124,58,237,0.2));
            border: 2px solid rgba(0,212,255,0.4);
            border-radius: 50px;
            font-weight: 700;
            font-size: 0.9rem;
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
            box-shadow: 0 8px 25px rgba(0,212,255,0.2);
        }

        .badge:hover {
            background: linear-gradient(145deg, rgba(0,212,255,0.4), rgba(124,58,237,0.4));
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,212,255,0.4);
        }

        /* Sections */
        .section {
            margin: 80px 0;
            padding: 50px 0;
        }

        .section-title {
            font-family: 'Orbitron', monospace;
            font-size: clamp(1.8rem, 4vw, 2.5rem);
            text-align: center;
            margin-bottom: 40px;
            background: linear-gradient(45deg, #00d4ff, #7c3aed);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, #00d4ff, #7c3aed);
            border-radius: 2px;
        }

        /* ASCII Boxes */
        .ascii-box {
            background: rgba(10,15,26,0.9);
            border: 2px solid rgba(0,212,255,0.5);
            border-radius: 15px;
            padding: 30px;
            margin: 20px 0;
            font-family: 'Courier New', monospace;
            font-size: 0.85rem;
            box-shadow: 0 15px 40px rgba(0,0,0,0.5);
            overflow-x: auto;
            backdrop-filter: blur(10px);
        }

        /* Tables */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: rgba(26,26,46,0.8);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 15px 40px rgba(0,0,0,0.4);
        }

        th, td {
            padding: 20px;
            text-align: left;
            border-bottom: 1px solid rgba(0,212,255,0.2);
        }

        th {
            background: linear-gradient(135deg, rgba(0,212,255,0.3), rgba(124,58,237,0.3));
            font-weight: 700;
            color: #00d4ff;
        }

        tr:hover {
            background: rgba(0,212,255,0.1);
            transform: scale(1.01);
        }

        /* Code Blocks */
        .code-block {
            background: rgba(0,0,0,0.7);
            border: 1px solid rgba(0,212,255,0.4);
            border-radius: 10px;
            padding: 25px;
            margin: 20px 0;
            font-family: 'Share Tech Mono', monospace;
            font-size: 0.9rem;
            position: relative;
            overflow: hidden;
        }

        .code-block::before {
            content: '⟨ Verilog ⟩';
            position: absolute;
            top: 10px;
            right: 15px;
            background: rgba(0,212,255,0.2);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.75rem;
            color: #00d4ff;
        }

        /* Stats Cards */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }

        .stat-card {
            background: linear-gradient(145deg, rgba(10,15,26,0.95), rgba(26,47,42,0.95));
            border: 2px solid rgba(0,212,255,0.4);
            border-radius: 20px;
            padding: 40px 30px;
            text-align: center;
            transition: all 0.4s ease;
            box-shadow: 0 20px 60px rgba(0,0,0,0.5);
            backdrop-filter: blur(15px);
        }

        .stat-card:hover {
            transform: translateY(-15px) scale(1.02);
            border-color: #00d4ff;
            box-shadow: 0 30px 80px rgba(0,212,255,0.4);
        }

        .stat-icon {
            font-size: 4rem;
            margin-bottom: 20px;
            background: linear-gradient(45deg, #00d4ff, #7c3aed);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* GitHub Stats */
        .github-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
            gap: 30px;
            margin: 50px 0;
        }

        /* Contact */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            margin: 40px 0;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 20px;
            background: rgba(10,15,26,0.8);
            border: 2px solid rgba(0,212,255,0.3);
            border-radius: 15px;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .contact-item:hover {
            border-color: #00d4ff;
            background: rgba(0,212,255,0.1);
            transform: translateY(-5px);
        }

        .contact-icon {
            font-size: 2rem;
            background: linear-gradient(45deg, #00d4ff, #7c3aed);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            width: 50px;
            text-align: center;
        }

        /* Footer */
        .footer {
            text-align: center;
            padding: 60px 0 40px;
            border-top: 2px solid rgba(0,212,255,0.3);
            margin-top: 80px;
        }

        .quote {
            font-size: 1.3rem;
            font-style: italic;
            margin: 30px 0;
            color: #ffd700;
            text-shadow: 0 0 20px rgba(255,215,0,0.5);
            font-family: 'Orbitron', monospace;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .container { padding: 0 15px; }
            .section { margin: 60px 0; padding: 30px 0; }
            .banner-slide { gap: 20px; font-size: 1.8rem; }
            .stats-grid { grid-template-columns: 1fr; }
            .github-stats { grid-template-columns: 1fr; }
        }

        /* Scroll Progress */
        .progress-bar {
            position: fixed;
            top: 0;
            left: 0;
            width: 0%;
            height: 4px;
            background: linear-gradient(90deg, #00d4ff, #7c3aed, #ff4d4d);
            z-index: 1000;
            transition: width 0.1s ease;
        }

        /* Particles Background */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: rgba(0,212,255,0.6);
            border-radius: 50%;
            animation: float 6s infinite linear;
        }

        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="progress-bar" id="progressBar"></div>
    <div class="particles" id="particles"></div>

    <div class="container">
        <!-- Header -->
        <header class="header">
            <h1 class="name-title">SAHIL MAURYA</h1>
            <p class="subtitle">
                <i class="fas fa-graduation-cap"></i> Research Scholar | IIT Mandi | 
                <i class="fas fa-microchip"></i> PQC Hardware Architect
            </p>
        </header>

        <!-- Tech Banner -->
        <div class="tech-banner">
            <div class="banner-slides">
                <div class="banner-slide">
                    <span>🔐</span>
                    <span>POST-QUANTUM CRYPTOGRAPHY</span>
                    <span>⚡</span>
                </div>
                <div class="banner-slide">
                    <span>🖥️</span>
                    <span>RISC-V SoC ARCHITECTURE</span>
                    <span>⚙️</span>
                </div>
                <div class="banner-slide">
                    <span>💾</span>
                    <span>DIGITAL VLSI DESIGN</span>
                    <span>🔌</span>
                </div>
                <div class="banner-slide">
                    <
