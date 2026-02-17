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

        .bg-wrapper {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            /* Ultra-smooth gradient mit sehr nahen Farbwerten */
            background: linear-gradient(-45deg, 
                #020205, #04040a, #070714, #0a0a1a, 
                #0d1120, #0a0a1a, #070714, #04040a, #020205);
            background-size: 400% 400%;
            animation: ultraGradient 30s ease-in-out infinite;
        }

        /* Anti-Banding Dither Overlay */
        .bg-wrapper::after {
            content: "";
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            opacity: 0.03;
            pointer-events: none;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
        }

        @keyframes ultraGradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.01);
            backdrop-filter: blur(35px);
            -webkit-backdrop-filter: blur(35px);
            border: 1px solid rgba(255, 255, 255, 0.05);
            border-radius: 40px;
            padding: 70px;
            text-align: center;
            box-shadow: 0 40px 120px rgba(0, 0, 0, 0.9);
            max-width: 600px;
            width: 90%;
        }

        h1 {
            color: #00d4ff;
            font-size: 4rem;
            margin: 0 0 10px 0;
            letter-spacing: -2px;
            text-shadow: 0 0 40px rgba(0, 212, 255, 0.3);
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
            border: 1px solid rgba(0, 212, 255, 0.3);
            border-radius: 100px;
            transition: all 0.5s cubic-bezier(0.15, 0.83, 0.66, 1);
            background: rgba(0, 212, 255, 0.01);
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
    <div class="bg-wrapper"></div>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>
        <div class="id-badge">Namespace Anchor: timiitzgit.github.io</div>
    </div>
</body>
</html>
