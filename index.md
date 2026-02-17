---
layout: null
---
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>Timiitz's Homepage</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            background: linear-gradient(-45deg, #050505, #1a1a2e, #16213e, #0f3460);
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', Roboto, sans-serif;
        }

        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 24px;
            padding: 50px;
            text-align: center;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
            max-width: 500px;
            width: 90%;
        }

        h1 {
            color: #00d4ff;
            font-size: 3.5rem;
            margin: 0 0 10px 0;
            text-shadow: 0 0 20px rgba(0, 212, 255, 0.4);
        }

        p {
            color: #adb5bd;
            font-size: 1.1rem;
            margin-bottom: 30px;
        }

        .link-btn {
            display: inline-block;
            color: #00d4ff;
            text-decoration: none;
            font-weight: bold;
            padding: 12px 30px;
            border: 2px solid #00d4ff;
            border-radius: 50px;
            transition: all 0.3s ease;
        }

        .link-btn:hover {
            background: #00d4ff;
            color: #050505;
            box-shadow: 0 0 20px rgba(0, 212, 255, 0.6);
            transform: translateY(-2px);
        }

        .id-badge {
            margin-top: 40px;
            font-size: 0.85rem;
            color: #555;
            letter-spacing: 1px;
            text-transform: uppercase;
        }
    </style>
</head>
<body>
    <div class="glass-card">
        <h1>Timiitz</h1>
        <p>Official Gateway for Technical Verification</p>
        
        <a href="https://github.com/TimiitzGit" class="link-btn">View GitHub Profile</a>

        <div class="id-badge">
            Namespace: timiitzgit.github.io
        </div>
    </div>
</body>
</html>
