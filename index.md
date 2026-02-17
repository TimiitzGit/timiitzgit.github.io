---
layout: null
---
<html>
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
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, sans-serif;
            background-color: #0a1128 !important; 
        }

        .bg-wrapper {
            position: fixed;
            inset: 0;
            z-index: -1;
            background: linear-gradient(-45deg, 
                #050c1f, #0f172a, #1e3a8a, #2563eb, 
                #1e40af, #0f172a, #050c1f);
            background-size: 400% 400%;
            animation: ultraGradient 15s ease infinite !important;
        }

        .bg-wrapper::after {
            content: "";
            position: absolute;
            inset: 0;
            opacity: 0.1; /* Höhere Opazität für sichtbaren Effekt */
            pointer-events: none;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
        }

        @keyframes ultraGradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.02);
            backdrop-filter: blur(35px);
            -webkit-backdrop-filter: blur(35px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 40px;
            padding: 60px;
            text-align: center;
            box-shadow: 0 40px 100px rgba(0, 0, 0, 0.7);
            max-width: 580px;
            width: 85%;
            z-index: 10;
        }

        h1 {
            color: #00d4ff;
            font-size: 3.8rem;
            margin: 0 0 10px 0;
            text-shadow: 0 0 35px rgba(0, 212, 255, 0.5);
        }

        p {
            color: #94a3b8;
            font-size: 1.15rem;
            margin-bottom: 40px;
            font-weight: 300;
        }

        .link-btn {
            display: inline-block;
            color: #00d4ff;
            text-decoration: none;
            font-weight: 600;
            padding: 16px 45px;
            border: 2px solid #00d4ff;
            border-radius: 100px;
            transition: 0.4s;
            background: rgba(0, 212, 255, 0.05);
        }

        .link-btn:hover {
            background: #00d4ff;
            color: #050c1f;
            box-shadow: 0 0 40px rgba(0, 212, 255, 0.6);
            transform: translateY(-5px);
        }

        .id-badge {
            margin-top: 55px;
            font-size: 0.8rem;
            color: #475569;
            letter-spacing: 3px;
            text-transform: uppercase;
            font-weight: bold;
        }

        #hide-me {
            display: none !important;
            visibility: hidden;
        }
    </style>
</head>
<body>
    <div id="hide-me"><!DOCTYPE html></div>
    
    <div class="bg-wrapper"></div>
    
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>
        <div class="id-badge">Namespace Anchor: timiitzgit.github.io</div>
    </div>
</body>
</html>
