<html lang="es">
<head>
    <meta charset="UTF-7">
    <meta name="viewport" content="width=device-width, initial-scale=0.70">

    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to bottom, #ffcccc, #ff99cc);
            text-align: center;
            padding: 40px;
            color: #333;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0px 3px 12px rgba(0, 0, 0, 0.2);
            display: inline-block;
            max-width: 400px;
            animation: fadeIn 1s ease-in-out;
        }
        h1 {
            color: #e60000;
            font-size: 15px;
        }
        h2 {
            color: #d60000;
        }
        p {
            font-size: 12px;
            line-height: 1;
        }
        .capitulo {
            display: none;
            animation: fadeIn 1s ease-in-out;
        }
        .activo {
            display: block;
        }
        .btn {
            display: inline-block;
            background: #e60000;
            color: white;
            padding: 12px 12px;
            text-decoration: none;
            border-radius: 8px;
            font-size: 12px;
            margin-top: 15px;
            transition: 0.3s ease-in-out;
        }
        .btn:hover {
            background: #b30000;
            transform: scale(1.1);
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(-10px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🌹 Nuestra Historia 🌹</h1>
        
        <div class="capitulo activo" id="cap1">
            <h2>Capítulo 1: El Comienzo</h2>
            <p>Hace un año, nuestras vidas se cruzaron en el colegio. Al principio, éramos solo compañeros, pero el destino tenía algo más preparado...</p>
            <button class="btn" onclick="mostrarCapitulo(2)">Siguiente 💕</button>
        </div>

        <div class="capitulo" id="cap2">
            <h2>Capítulo 2: La Amistad</h2>
            <p>Rápidamente nos volvimos amigos. Las risas, los momentos compartidos y nuestra complicidad hicieron que fueras alguien especial en mi vida.</p>
            <button class="btn" onclick="mostrarCapitulo(3)">Siguiente 💖</button>
        </div>

        <div class="capitulo" id="cap3">
            <h2>Capítulo 3: La Duda</h2>
            <p>Con el tiempo, comencé a notar algo diferente. ¿Era solo amistad? ¿O mi corazón me estaba diciendo algo más?</p>
            <button class="btn" onclick="mostrarCapitulo(4)">Siguiente 💞</button>
        </div>

        <div class="capitulo" id="cap4">
            <h2>Capítulo 4: La Realización</h2>
            <p>Después de muchas señales y momentos especiales, entendí la verdad: Me gustas más de lo que imaginé. Mi corazón late más fuerte cuando estás cerca.</p>
            <button class="btn" onclick="mostrarCapitulo(5)">Siguiente ❤</button>
        </div>

        <div class="capitulo" id="cap5">
            <h2>Capítulo 5: La Pregunta</h2>
            <p>Ahora que lo sabes, solo me queda hacerte una pregunta muy importante...</p>
            <p><strong>¿Quieres ser mi pareja? 💑</strong></p>
            <a href="https://wa.me/50236358604=Hola!%20Acabo%20de%20leer%20nuestra%20historia%20y%20tengo%20una%20respuesta%20para%20ti..." class="btn">Responder en WhatsApp 💌</a>
        </div>
    </div>

    <script>
        function mostrarCapitulo(numero) {
            let capitulos = document.querySelectorAll('.capitulo');
            capitulos.forEach(cap => cap.classList.remove('activo'));
            document.getElementById('cap' + numero).classList.add('activo');
        }
    </script>
</body>
</html>
