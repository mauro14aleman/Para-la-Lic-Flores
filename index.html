<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz San Valentín</title>
    <style>
        body {
            background-color: #ffe6f2; /* Rosa claro */
            font-family: Arial, sans-serif;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden; /* Para que los corazones no generen scroll */
        }

        .carta-contenedor {
            position: relative;
            cursor: pointer;
        }

        .carta {
            background-color: white;
            border: 2px solid #ffb3c6; /* Borde rosa más fuerte */
            width: 300px;
            height: 200px;
            border-radius: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 1.5em;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.5s ease; /* Transición suave para abrir la carta */
            transform-origin: top center; /* Punto de origen para la rotación */
        }

        .carta.abierta {
            transform: rotateX(-180deg); /* Rota para simular que se abre */
            opacity: 0; /* Para que la carta cerrada desaparezca */
            visibility: hidden; /* Oculta completamente para que no interfiera */
        }

        .dedicatoria {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.9); /* Fondo blanco semi-transparente */
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            opacity: 0;
            visibility: hidden;
            transition: opacity 1s ease 0.5s, visibility 0s linear 0.5s; /* Retraso para que aparezca después de abrir la carta */
            pointer-events: none; /* Para que no interfiera con clics después de abrir */
            max-height: 70vh; /* Altura máxima de la dedicatoria */
            overflow-y: auto; /* Permite el scroll vertical si el contenido excede la altura */
            display: flex; /* Para alinear verticalmente el botón */
            flex-direction: column; /* Para apilar el texto y el botón */
            justify-content: space-between; /* Espacio entre texto y botón */
        }

        .dedicatoria.mostrar {
            opacity: 1;
            visibility: visible;
            pointer-events: auto; /* Vuelve a habilitar los eventos si fuera necesario */
        }

        .boton-sorpresa {
            padding: 10px 20px;
            background-color: #ffb3c6; /* Rosa fuerte para el botón */
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            transition: background-color 0.3s ease;
            align-self: center; /* Centra el botón horizontalmente dentro de la dedicatoria */
            margin-top: 15px; /* Espacio entre el texto y el botón */
        }

        .boton-sorpresa:hover {
            background-color: #ff80a3; /* Rosa más oscuro al pasar el ratón */
        }

        .carta-sorpresa {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: #f0e6ff; /* Morado claro */
            border: 2px solid #d8bfff; /* Borde morado más fuerte */
            width: 300px;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            font-size: 1.2em;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            visibility: hidden; /* Inicialmente oculta */
            opacity: 0;
            transition: opacity 0.5s ease, visibility 0s linear 0.5s; /* Transición suave al aparecer */
            pointer-events: none; /* Inicialmente no interactiva */
        }

        .carta-sorpresa.mostrar-carta {
            visibility: visible; /* Hace visible la carta sorpresa */
            opacity: 1; /* Muestra la carta sorpresa */
            pointer-events: auto; /* Vuelve a habilitar los eventos si fuera necesario */
        }


        .corazones-contenedor {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none; /* Para que no interfiera con clics */
        }

        .corazon {
            position: absolute;
            font-size: 1.5em;
            color: red;
            animation: caerCorazon 5s linear infinite; /* Animación para caer */
            opacity: 0; /* Inicialmente transparentes */
        }

        @keyframes caerCorazon {
            0% {
                transform: translateY(-100vh) translateX(0); /* Empieza arriba */
                opacity: 0;
            }
            10% {
                opacity: 1; /* Empiezan a aparecer */
            }
            80% {
                opacity: 1; /* Visibles durante la caída */
            }
            100% {
                transform: translateY(100vh) translateX(0); /* Termina abajo */
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="carta-contenedor" id="cartaContenedor">
        <div class="carta" id="carta">
            Toca aquí
        </div>
        <div class="dedicatoria" id="dedicatoria">
            <p id="textoDedicatoria">
                [Aquí va tu dedicatoria para tu novia.  Escribe algo muy bonito y especial para ella.]
            </p>
            <button class="boton-sorpresa" id="botonSorpresa">Púlsame</button>
        </div>
    </div>
    <div class="carta-sorpresa" id="cartaSorpresa">
        Eres la persona con quien quiero aprender a amar los días las noches los buenos y malos momentos
    </div>
    <div class="corazones-contenedor" id="corazonesContenedor">
        </div>

    <script>
        const cartaContenedor = document.getElementById('cartaContenedor');
        const carta = document.getElementById('carta');
        const dedicatoria = document.getElementById('dedicatoria');
        const textoDedicatoria = document.getElementById('textoDedicatoria');
        const corazonesContenedor = document.getElementById('corazonesContenedor');
        const botonSorpresa = document.getElementById('botonSorpresa');
        const cartaSorpresa = document.getElementById('cartaSorpresa');


        // *** ¡Aquí debes escribir tu dedicatoria! ***
        const miDedicatoria = `
            Mi amada novia,

            Feliz 14 de febrero.  Cada díaestando lejos de ti es una tortura sin embargo eso me hace amar mas el escribirte el escucharte para mi es una aventura maravillosa y llena de alegría saber que pronto te tendre entre mis brazos y recostada en mi pecho .  Eres la persona más increíble que conozco y estoy muy agradecido de tenerte en mi vida.

            Porque dada la inmensidad del tiempo y la inmensidad del universo, es un placer inmenso compartir un planeta y un tiempo contigo.

            Con todo mi amor,
            Mauricio que orgullosamente es tu novio.

            P.D. Espero que te guste esta sorpresa especial que prepare para ti con mucho amor y cariño.  Cada detalle está pensado en ti.  Eres mi inspiración.
        `;
        textoDedicatoria.innerText = miDedicatoria; // Insertamos la dedicatoria en el HTML

        let cartaAbierta = false; // Variable para controlar si la carta está abierta

        cartaContenedor.addEventListener('click', () => {
            if (!cartaAbierta) {
                carta.classList.add('abierta'); // Añade la clase 'abierta' para la animación
                dedicatoria.classList.add('mostrar'); // Muestra la dedicatoria
                generarCorazones(); // Genera los corazones
                cartaAbierta = true; // Marca la carta como abierta
            }
        });

        botonSorpresa.addEventListener('click', (event) => {
            event.stopPropagation(); // Evita que el clic en el botón también cierre la carta sorpresa si el contenedor es el mismo
            dedicatoria.classList.remove('mostrar'); // Oculta la dedicatoria inicial
            cartaSorpresa.classList.add('mostrar-carta'); // Muestra la carta sorpresa morada
        });

        cartaSorpresa.addEventListener('click', () => {
            cartaSorpresa.classList.remove('mostrar-carta'); // Oculta la carta sorpresa morada al hacer clic en ella
            dedicatoria.classList.add('mostrar'); // Vuelve a mostrar la dedicatoria inicial
        });


        function generarCorazones() {
            for (let i = 0; i < 50; i++) { // Genera 50 corazones
                const corazon = document.createElement('div');
                corazon.classList.add('corazon');
                corazon.textContent = '❤️'; // Emoji de corazón
                corazon.style.left = `${Math.random() * 100}%`; // Posición horizontal aleatoria
                corazon.style.animationDelay = `${Math.random() * 2}s`; // Retardo aleatorio para que no caigan todos juntos
                corazon.style.animationDuration = `${5 + Math.random() * 3}s`; // Duración ligeramente aleatoria
                corazonesContenedor.appendChild(corazon);
            }
        }
    </script>
</body>
</html>
