---
layout: null
---
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>Timiitz / TimiitzGit</title>
    <style>
        * { box-sizing: border-box; }
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            background-color: #020205;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, sans-serif;
        }

        .bg-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: #020205;
        }

        .gradient-sphere {
            position: absolute;
            width: 150vmax;
            height: 150vmax;
            top: -25%;
            left: -25%;
            background: radial-gradient(circle at center, 
                rgba(26, 26, 46, 0.8) 0%, 
                rgba(15, 52, 96, 0.4) 30%, 
                rgba(10, 25, 47, 0.2) 60%, 
                transparent 100%);
            animation: rotate 35s linear infinite;
            filter: blur(80px);
        }

        .noise-overlay {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            opacity: 0.06;
            pointer-events: none;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
        }

        @keyframes rotate {
            from { transform: rotate(0deg) scale(1); }
            50% { transform: rotate(180deg) scale(1.1); }
            to { transform: rotate(360deg) scale(1); }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.015);
            backdrop-filter: blur(40px);
            -webkit-backdrop-filter: blur(40px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 40px;
            padding: 70px;
            text-align: center;
            box-shadow: 0 40px 120px rgba(0, 0, 0, 0.9);
            max-width: 600px;
            width: 90%;
            z-index: 10;
        }

        h1 {
            color: #00d4ff;
            font-size: 4rem;
            margin: 0 0 10px 0;
            letter-spacing: -2px;
            text-shadow: 0 0 40px rgba(0, 212, 255, 0.4);
        }

        p {
            color: #64748b;
            font-size: 1.2rem;
            margin-bottom: 45px;
            font-weight: 300;
        }

        .link-btn {
            display: inline-block;
            color: #00d4ff;
            text-decoration: none;
            font-weight: 600;
            padding: 18px 50px;
            border: 1px solid rgba(0, 212, 255, 0.4);
            border-radius: 100px;
            transition: all 0.5s cubic-bezier(0.15, 0.83, 0.66, 1);
            background: rgba(0, 212, 255, 0.02);
        }

        .link-btn:hover {
            background: #00d4ff;
            color: #020205;
            box-shadow: 0 0 50px rgba(0, 212, 255, 0.5);
            transform: translateY(-5px);
        }

        .id-badge {
            margin-top: 65px;
            font-size: 0.8rem;
            color: #334155;
            letter-spacing: 4px;
            text-transform: uppercase;
            font-weight: 700;
        }
    </style>
</head>
<body>
    <div class="bg-container">
        <div class="gradient-sphere"></div>
        <div class="noise-overlay"></div>
    </div>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>
        <div class="id-badge">Namespace Anchor: timiitzgit.github.io</div>
    </div>
</body>
</html>
