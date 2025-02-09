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
        .heart-animation {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
            pointer-events: none;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: red;
            clip-path: polygon(50% 0%, 100% 35%, 85% 100%, 50% 80%, 15% 100%, 0% 35%);
            opacity: 0.8;
            animation: float 3s linear infinite;
        }
        @keyframes float {
            0% {
                transform: translateY(0) scale(1);
                opacity: 1;
            }
            100% {
                transform: translateY(-100vh) scale(1.5);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="heart-animation"></div>
    <h1>Mi amada novia Jensi, lamento si de alguna manera siempre causo disgustos en tu persona. 💛</h1>
    <p>Eres mi paz, mi amor y mi refugio. Nada cambiará cuánto te quiero. Lo que más deseo es hacerte muy feliz y que sientas lo importante que eres para mí. 💖</p>
    <p>Siempre estaré aquí para ti, pase lo que pase. Tú eres mi hogar. 🏡💕</p>
    <div class="video-container">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/yl3GDni9WCQ?autoplay=1" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
    <script>
        function createHeart() {
            let heart = document.createElement("div");
            heart.className = "heart";
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.backgroundColor = ["#ff0000", "#6a0dad", "#4682b4"][Math.floor(Math.random() * 3)];
            document.querySelector(".heart-animation").appendChild(heart);
            setTimeout(() => heart.remove(), 3000);
        }
        setInterval(createHeart, 500);
    </script>
</body>
</html>

        
        document.body.addEventListener("click", createHeart);
    </script>
</body>
</html>

</html>
