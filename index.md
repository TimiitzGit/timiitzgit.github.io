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
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, sans-serif;
            background: #0a192f;
        }

        .bg-mesh {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background-color: #0a192f;
            background-image: 
                radial-gradient(at 0% 0%, rgba(26, 60, 100, 0.8) 0, transparent 50%), 
                radial-gradient(at 50% 0%, rgba(16, 44, 84, 0.8) 0, transparent 50%), 
                radial-gradient(at 100% 0%, rgba(30, 58, 138, 0.8) 0, transparent 50%), 
                radial-gradient(at 0% 50%, rgba(15, 23, 42, 0.8) 0, transparent 50%), 
                radial-gradient(at 100% 50%, rgba(29, 78, 216, 0.4) 0, transparent 50%), 
                radial-gradient(at 0% 100%, rgba(30, 58, 138, 0.8) 0, transparent 50%), 
                radial-gradient(at 50% 100%, rgba(15, 23, 42, 0.8) 0, transparent 50%), 
                radial-gradient(at 100% 100%, rgba(26, 60, 100, 0.8) 0, transparent 50%);
            background-size: 200% 200%;
            animation: meshFlow 15s ease infinite;
        }

        .noise {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            opacity: 0.08;
            pointer-events: none;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
        }

        @keyframes meshFlow {
            0% { background-position: 0% 0%; }
            50% { background-position: 100% 100%; }
            100% { background-position: 0% 0%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(25px);
            -webkit-backdrop-filter: blur(25px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 35px;
            padding: 60px;
            text-align: center;
            box-shadow: 0 25px 80px rgba(0, 0, 0, 0.6);
            max-width: 580px;
            width: 85%;
            z-index: 10;
        }

        h1 {
            color: #00d4ff;
            font-size: 3.8rem;
            margin: 0 0 10px 0;
            text-shadow: 0 0 30px rgba(0, 212, 255, 0.4);
        }

        p {
            color: #94a3b8;
            font-size: 1.15rem;
            margin-bottom: 40px;
        }

        .link-btn {
            display: inline-block;
            color: #00d4ff;
            text-decoration: none;
            font-weight: 600;
            padding: 16px 45px;
            border: 2px solid #00d4ff;
            border-radius: 50px;
            transition: 0.3s;
            background: rgba(0, 212, 255, 0.05);
        }

        .link-btn:hover {
            background: #00d4ff;
            color: #0a192f;
            box-shadow: 0 0 30px rgba(0, 212, 255, 0.6);
            transform: translateY(-3px);
        }

        .id-badge {
            margin-top: 50px;
            font-size: 0.8rem;
            color: #475569;
            letter-spacing: 3px;
            text-transform: uppercase;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="bg-mesh"></div>
    <div class="noise"></div>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>
        <div class="id-badge">Namespace Anchor: timiitzgit.github.io</div>
    </div>
</body>
</html>
