<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(120deg, #ff9a9e, #fad0c4);
            animation: backgroundAnimation 10s ease infinite;
            font-family: 'Arial', sans-serif;
            color: #fff;
            overflow: hidden;
        }
        @keyframes backgroundAnimation {
            0% { background: linear-gradient(120deg, #ff9a9e, #fad0c4); }
            50% { background: linear-gradient(120deg, #fad0c4, #ff9a9e); }
            100% { background: linear-gradient(120deg, #ff9a9e, #fad0c4); }
        }
        .container {
            text-align: center;
            position: relative;
            animation: fadeIn 2s ease-in-out;
        }
        h1 {
            font-size: 4em;
            margin: 0;
            text-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        p {
            font-size: 1.5em;
            margin-top: 20px;
            text-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
        }
        .balloons {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }
        .balloon {
            position: absolute;
            bottom: -100px;
            width: 50px;
            height: 70px;
            background: radial-gradient(circle, #fff, #ff6b6b);
            border-radius: 50% 50% 50% 50%;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            animation: float 5s ease-in infinite;
            transition: transform 0.3s;
        }
        .balloon:hover {
            transform: scale(1.1);
        }
        @keyframes float {
            0% {
                transform: translateY(0);
                opacity: 1;
            }
            100% {
                transform: translateY(-110vh);
                opacity: 0;
            }
        }
        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }
        .star {
            position: absolute;
            background: yellow;
            border-radius: 50%;
            animation: twinkle 1.5s infinite;
        }
        @keyframes twinkle {
            0%, 100% { opacity: 0.5; }
            50% { opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎉 Happy Birthday! 🎂</h1>
        <p>Wishing you a day filled with love and laughter!</p>
        <p>May all your dreams come true!</p>
        <p>Enjoy your special day!</p>
    </div>
    <div class="balloons">
        <!-- Balloons -->
        <div class="balloon" style="left: 10%; animation-duration: 6s; background: radial-gradient(circle, #ff6b6b, #ff9a9e);"></div>
        <div class="balloon" style="left: 25%; animation-duration: 7s; background: radial-gradient(circle, #ff9e6b, #ff6b9e);"></div>
        <div class="balloon" style="left: 50%; animation-duration: 5s; background: radial-gradient(circle, #6bff9e, #6b9eff);"></div>
        <div class="balloon" style="left: 75%; animation-duration: 6.5s; background: radial-gradient(circle, #9eff6b, #9e6bff);"></div>
        <div class="balloon" style="left: 90%; animation-duration: 8s; background: radial-gradient(circle, #6b6bff, #ff6b6b);"></div>
    </div>
    <div class="stars">
        <!-- Stars -->
        <div class="star" style="top: 10%; left: 20%; width: 10px; height: 10px;"></div>
        <div class="star" style="top: 15%; left: 50%; width: 8px; height: 8px;"></div>
        <div class="star" style="top: 5%; left: 80%; width: 12px; height: 12px;"></div>
        <div class="star" style="top: 25%; left: 30%; width: 6px; height: 6px;"></div>
        <div class="star" style="top: 20%; left: 70%; width: 9px; height: 9px;"></div>
    </div>
</body>
</html>
