<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Varsha & Bobby's Wedding</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;700&display=swap');
        body {
            font-family: 'Poppins', sans-serif;
            text-align: center;
            background: url('https://images.pexels.com/photos/459225/pexels-photo-459225.jpeg') no-repeat center center/cover;
            color: #fff;
            overflow: hidden;
        }
        header {
            background: rgba(139, 69, 19, 0.9);
            padding: 20px;
            color: gold;
            font-size: 35px;
            font-weight: bold;
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            font-family: 'Great Vibes', cursive;
        }
        section {
            margin: 20px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 15px;
            box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.2);
        }
        .countdown {
            font-size: 35px;
            margin-top: 20px;
            font-weight: bold;
            color: gold;
        }
        .animation {
            position: fixed;
            width: 100vw;
            height: 100vh;
            background: rgba(255, 215, 0, 0.8);
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 50px;
            color: brown;
            font-weight: bold;
            font-family: 'Great Vibes', cursive;
            animation: fadeOut 3s forwards;
            z-index: 1000;
        }
        @keyframes fadeOut {
            0% { opacity: 1; }
            100% { opacity: 0; visibility: hidden; }
        }
    </style>
</head>
<body>
    <div class="animation">शुभ विवाह - Varsha & Bobby</div>
    <header>💛 शुभ विवाह: Varsha & Bobby 💛</header>
    <section>
        <h2>🕉️ Save the Date - 29 अप्रैल! 🕉️</h2>
        <p>हमारे शुभ विवाह में आपका स्वागत है। कृपया हमें आशीर्वाद दें।</p>
        <p class="countdown" id="countdown"></p>
    </section>
    <script>
        function countdown() {
            const weddingDate = new Date("2025-04-29T00:00:00");
            const now = new Date();
            const diff = weddingDate - now;
            const days = Math.floor(diff / (1000 * 60 * 60 * 24));
            document.getElementById("countdown").innerText = days + " दिन शेष!";
        }
        countdown();
        setInterval(countdown, 86400000);
    </script>
</body>
</html>
