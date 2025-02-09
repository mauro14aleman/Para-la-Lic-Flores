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
        @keyframes glow {
            0% { text-shadow: 0 0 10px #ffcc00, 0 0 20px #ff9900; }
            100% { text-shadow: 0 0 20px #ffcc00, 0 0 30px #ff6600; }
        }
        .flowers {
            position: absolute;
            width: 100%;
            height: 100%;
        }
        .flower {
            position: absolute;
            width: 50px;
            height: 50px;
            background: url('https://i.imgur.com/jD4J26h.png'); /* Imagen de una flor amarilla */
            background-size: cover;
            animation: fall linear infinite;
        }
        @keyframes fall {
            0% { transform: translateY(-100px) rotate(0deg); }
            100% { transform: translateY(100vh) rotate(360deg); }
        }
        audio {
            display: none;
        }
    </style>
</head>
<body>
    <div class="flowers"></div>
    <h1>Lo siento, mi amor. Te amo más que nunca. 💛</h1>
    <audio autoplay loop>
        <source src="te-amo-y-mas.mp3" type="audio/mpeg">
        Tu navegador no soporta el audio.
    </audio>
    <script>
        function createFlowers() {
            for (let i = 0; i < 20; i++) {
                let flower = document.createElement("div");
                flower.className = "flower";
                flower.style.left = Math.random() * 100 + "vw";
                flower.style.animationDuration = (Math.random() * 3 + 2) + "s";
                document.querySelector(".flowers").appendChild(flower);
            }
        }
        createFlowers();
    </script>
</body>
</html>

