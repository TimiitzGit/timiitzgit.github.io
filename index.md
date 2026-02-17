---
layout: null
---
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>Timiitz / TimiitzGit</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, sans-serif;
            background: #050505;
        }

        .background-animate {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -2;
            background: linear-gradient(-45deg, #050505, #0a0a12, #1a1a2e, #16213e, #1a1a2e, #0f3460, #0a192f, #16213e, #050505);
            background-size: 400% 400%;
            animation: gradient 22s ease-in-out infinite;
        }

        .grain {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -1;
            opacity: 0.04;
            pointer-events: none;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3E%3C/svg%3E");
        }

        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.02);
            backdrop-filter: blur(25px);
            -webkit-backdrop-filter: blur(25px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 32px;
            padding: 70px;
            text-align: center;
            box-shadow: 0 30px 80px rgba(0, 0, 0, 0.7);
            max-width: 550px;
            width: 85%;
            z-index: 10;
        }

        h1 {
            color: #00d4ff;
            font-size: 3.8rem;
            margin: 0 0 10px 0;
            letter-spacing: -1px;
            text-shadow: 0 0 40px rgba(0, 212, 255, 0.4);
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
            padding: 16px 40px;
            border: 1.5px solid rgba(0, 212, 255, 0.4);
            border-radius: 60px;
            transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
            background: rgba(0, 212, 255, 0.02);
        }

        .link-btn:hover {
            background: #00d4ff;
            color: #050505;
            box-shadow: 0 0 30px rgba(0, 212, 255, 0.6);
            transform: translateY(-4px);
        }

        .id-badge {
            margin-top: 55px;
            font-size: 0.75rem;
            color: #475569;
            letter-spacing: 3px;
            text-transform: uppercase;
            font-weight: 600;
            opacity: 0.8;
        }
    </style>
</head>
<body>
    <div class="background-animate"></div>
    <div class="grain"></div>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>
        <div class="id-badge">Namespace Anchor: timiitzgit.github.io</div>
    </div>
</body>
</html>
