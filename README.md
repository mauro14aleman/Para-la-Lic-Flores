<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lo Siento, Mi Amor</title>
    <style>
        body {
            background-color: #121212;
            color: #ffd700;
            font-family: 'Pacifico', cursive;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 3rem;
            text-shadow: 0 0 10px #ffcc00, 0 0 20px #ff9900;
            animation: glow 1.5s infinite alternate;
        }
        p {
            font-size: 1.5rem;
            max-width: 80%;
            margin: 10px auto;
            color: #fff;
            text-shadow: 0 0 5px #ffd700;
        }
        @keyframes glow {
            0% { text-shadow: 0 0 10px #ffcc00, 0 0 20px #ff9900; }
            100% { text-shadow: 0 0 20px #ffcc00, 0 0 30px #ff6600; }
        }
        .flowers {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        .flower {
            position: absolute;
            width: 40px;
            height: 40px;
            background: url('https://i.imgur.com/9ZCAdK2.png');
            background-size: cover;
            animation: fall linear infinite;
        }
        @keyframes fall {
            0% { transform: translateY(-100px) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }
        .video-container {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="flowers"></div>
    <h1>Mi amada novia Jensi, lamento si de alguna manera siempre causo disgustos en tu persona. 💛</h1>
    <p>Eres mi paz, mi amor y mi refugio. Nada cambiará cuánto te quiero. Lo que más deseo es hacerte muy feliz y que sientas lo importante que eres para mí. 💖</p>
    <p>Siempre estaré aquí para ti, pase lo que pase. Tú eres mi hogar. 🏡💕</p>
    <div class="video-container">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/8vH9B-7-hr8?autoplay=1&mute=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
    <script>
        function createFlowers() {
            for (let i = 0; i < 20; i++) {
                let flower = document.createElement("div");
                flower.className = "flower";
                flower.style.left = Math.random() * 100 + "vw";
                flower.style.animationDuration = (Math.random() * 3 + 4) + "s";
                document.querySelector(".flowers").appendChild(flower);
            }
        }
        createFlowers();
    </script>
</body>
</html>
