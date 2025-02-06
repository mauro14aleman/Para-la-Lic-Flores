<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tarjeta Interactiva</title>
    <style>
        body {
            background: linear-gradient(to bottom right, #4F92C3, #F9D423); /* Azules y amarillos */
            color: white;
            font-family: 'Arial', sans-serif;
            text-align: center;
            padding: 50px;
            height: 100vh;
            margin: 0;
            overflow: hidden;
            position: relative;
        }

        h1 {
            font-size: 40px;
            margin: 0;
            padding: 20px;
        }

        .heart {
            position: absolute;
            font-size: 25px;
            animation: heartAnimation 1s ease-in-out forwards;
        }

        @keyframes heartAnimation {
            0% {
                transform: scale(1);
                opacity: 1;
            }
            100% {
                transform: scale(2);
                opacity: 0;
                top: -50px;
            }
        }

        .message {
            font-size: 20px;
            margin-top: 30px;
        }

        .message.hidden {
            display: none;
        }

        audio {
            display: none;
        }
    </style>
</head>
<body>

    <h1>Para mi amor Jensi, con todo mi cariño tratando de robarte una sonrisa ❤️</h1>
    <audio id="song" autoplay loop>
        <source src="https://www.example.com/RewriteTheStars.mp3" type="audio/mp3">
        Tu navegador no soporta este formato de audio.
    </audio>

    <div class="message" id="message1">
        <p>Hola, mi amor. Siempre estoy contigo, incluso cuando te sientas triste. 💙</p>
    </div>
    <div class="message hidden" id="message2">
        <p>Recuerda que siempre tienes una razón para sonreír, ¡te quiero mucho! 💛</p>
    </div>
    <div class="message hidden" id="message3">
        <p>No importa lo que pase, siempre estaré aquí para ti. 🌟</p>
    </div>

    <script>
        let currentMessage = 1;

        // Cambia el mensaje al hacer click
        document.body.addEventListener('click', function() {
            // Mostrar corazones
            let heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerText = '❤️';
            heart.style.left = `${Math.random() * window.innerWidth}px`;
            heart.style.top = `${Math.random() * window.innerHeight}px`;
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 1000); // Elimina el corazón después de 1 segundo

            // Cambia el mensaje
            if (currentMessage === 1) {
                document.getElementById('message1').classList.add('hidden');
                document.getElementById('message2').classList.remove('hidden');
                currentMessage = 2;
            } else if (currentMessage === 2) {
                document.getElementById('message2').classList.add('hidden');
                document.getElementById('message3').classList.remove('hidden');
                currentMessage = 3;
            } else {
                document.getElementById('message3').classList.add('hidden');
                document.getElementById('message1').classList.remove('hidden');
                currentMessage = 1;
            }
        });

        // Reproduce la canción automáticamente al cargar
        window.onload = function() {
            document.getElementById('song').play();
        };
    </script>

</body>
</html>
