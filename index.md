---
layout: null
---
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>Timiitz / TimiitzGit</title>
    <style>
        :root {
            --bg-color: #050505;
            --accent: #00d4ff;
            --deep-blue: #0a192f;
            --bright-blue: #1e40af;
        }

        * { box-sizing: border-box; }
        
        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            background-color: var(--bg-color);
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }

        .animated-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: linear-gradient(-45deg, 
                #050505, 
                #0a192f, 
                #1e3a8a, 
                #0f172a, 
                #020617);
            background-size: 400% 400%;
            animation: flow 15s ease infinite;
        }

        .animated-bg::after {
            content: "";
            position: absolute;
            inset: 0;
            opacity: 0.05;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
            pointer-events: none;
        }

        @keyframes flow {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.02);
            backdrop-filter: blur(25px);
            -webkit-backdrop-filter: blur(25px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 30px;
            padding: 60px;
            text-align: center;
            box-shadow: 0 25px 60px rgba(0, 0, 0, 0.7);
            max-width: 550px;
            width: 90%;
            z-index: 10;
        }

        h1 {
            color: var(--accent);
            font-size: 3.5rem;
            margin: 0 0 10px 0;
            text-shadow: 0 0 25px rgba(0, 212, 255, 0.4);
        }

        p {
            color: #94a3b8;
            font-size: 1.1rem;
            margin-bottom: 40px;
        }

        .link-btn {
            display: inline-block;
            color: var(--accent);
            text-decoration: none;
            font-weight: 600;
            padding: 15px 40px;
            border: 2px solid var(--accent);
            border-radius: 50px;
            transition: all 0.3s ease;
            background: rgba(0, 212, 255, 0.05);
        }

        .link-btn:hover {
            background: var(--accent);
            color: #050505;
            box-shadow: 0 0 30px rgba(0, 212, 255, 0.5);
            transform: translateY(-3px);
        }

        .id-badge {
            margin-top: 50px;
            font-size: 0.75rem;
            color: #475569;
            letter-spacing: 3px;
            text-transform: uppercase;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="animated-bg"></div>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>
        <div class="id-badge">Namespace Anchor: timiitzgit.github.io</div>
    </div>
</body>
</html>
