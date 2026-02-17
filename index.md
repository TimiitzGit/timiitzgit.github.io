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
            background: linear-gradient(-45deg, #050505, #1a1a2e, #0a192f, #16213e, #0f3460, #090909);
            background-size: 400% 400%;
            animation: gradient 18s ease-in-out infinite;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.02);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 28px;
            padding: 60px;
            text-align: center;
            box-shadow: 0 25px 60px rgba(0, 0, 0, 0.6);
            max-width: 550px;
            width: 85%;
        }

        h1 {
            color: #00d4ff;
            font-size: 3.8rem;
            margin: 0 0 15px 0;
            letter-spacing: -1px;
            text-shadow: 0 0 30px rgba(0, 212, 255, 0.3);
        }

        p {
            color: #94a3b8;
            font-size: 1.15rem;
            margin-bottom: 35px;
            font-weight: 300;
        }

        .link-btn {
            display: inline-block;
            color: #00d4ff;
            text-decoration: none;
            font-weight: 600;
            padding: 14px 35px;
            border: 1.5px solid rgba(0, 212, 255, 0.5);
            border-radius: 50px;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            background: rgba(0, 212, 255, 0.03);
        }

        .link-btn:hover {
            background: #00d4ff;
            color: #050505;
            box-shadow: 0 0 25px rgba(0, 212, 255, 0.5);
            transform: translateY(-3px);
            border-color: #00d4ff;
        }

        .id-badge {
            margin-top: 50px;
            font-size: 0.75rem;
            color: #475569;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-weight: 600;
        }
    </style>
</head>
<body>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway-Domain for Technical Verification</p>
        
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>

        <div class="id-badge">
            Namespace Anchor: timiitzgit.github.io
        </div>
    </div>
</body>
</html>
