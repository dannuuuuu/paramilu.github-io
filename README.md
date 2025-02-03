# paramilu.github-io
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            color: #d63384;
            margin: 0;
            padding: 20px;
        }
        .container {
            margin-top: 50px;
        }
        h1 {
            font-size: 2.5em;
        }
        p {
            font-size: 1.3em;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 1.2em;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: #ff4081;
            color: white;
        }
        .no {
            background-color: #888;
            color: white;
        }
        .yes:hover {
            background-color: #e91e63;
        }
        .no:hover {
            background-color: #666;
        }
        #heart {
            font-size: 50px;
            animation: heartbeat 1.5s infinite;
        }
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>💖 ¿Quieres ser mi San Valentín? 💖</h1>
        <p>Eres la persona más especial para mí y me encantaría compartir este día contigo. 💕</p>
        <div class="buttons">
            <button class="yes" onclick="respuesta('sí')">Sí 💘</button>
            <button class="no" id="noButton" onmouseover="moverBoton()">No 😢</button>
        </div>
        <p id="mensaje"></p>
    </div>

    <script>
        function respuesta(opcion) {
            if (opcion === 'sí') {
                document.getElementById("mensaje").innerHTML = "🥰 ¡Sabía que dirías que sí! ¡Eres lo mejor que me ha pasado! ❤💖";
            }
        }

        function moverBoton() {
            let noButton = document.getElementById("noButton");
            let x = Math.random() * (window.innerWidth - 150);
            let y = Math.random() * (window.innerHeight - 100);
            noButton.style.position = "absolute";
            noButton.style.left = ${x}px;
            noButton.style.top = ${y}px;
        }
    </script>
</body>
</html>
