<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nuestra Historia</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffe6e6;
            text-align: center;
            padding: 50px;
        }
        .container {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
            max-width: 600px;
        }
        h1 {
            color: #e60000;
        }
        .capitulo {
            display: none;
        }
        .activo {
            display: block;
        }
        .btn {
            display: inline-block;
            background-color: #e60000;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            font-size: 20px;
            margin-top: 20px;
            cursor: pointer;
        }
        .btn:hover {
            background-color: #b30000;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Nuestra Historia</h1>
        
        <div class="capitulo activo" id="cap1">
            <h2>Capítulo 1: El Comienzo</h2>
            <p>Todo comenzó hace un año, cuando nos conocimos en el colegio. Al principio, éramos solo compañeros, pero algo cambió...</p>
            <button class="btn" onclick="mostrarCapitulo(2)">Siguiente</button>
        </div>

        <div class="capitulo" id="cap2">
            <h2>Capítulo 2: La Amistad</h2>
            <p>Con el tiempo, nuestra amistad creció. Las risas, las charlas y los momentos compartidos hicieron que fueras alguien especial en mi vida.</p>
            <button class="btn" onclick="mostrarCapitulo(3)">Siguiente</button>
        </div>

        <div class="capitulo" id="cap3">
            <h2>Capítulo 3: La Duda</h2>
            <p>Empecé a darme cuenta de que cada vez me importabas más. Me preguntaba si solo era amistad o si había algo más en mi corazón.</p>
            <button class="btn" onclick="mostrarCapitulo(4)">Siguiente</button>
        </div>

        <div class="capitulo" id="cap4">
            <h2>Capítulo 4: La Realización</h2>
            <p>Después de muchas señales y emociones, entendí la verdad: Me gustas más de lo que imaginé.</p>
            <button class="btn" onclick="mostrarCapitulo(5)">Siguiente</button>
        </div>

        <div class="capitulo" id="cap5">
            <h2>Capítulo 5: La Pregunta</h2>
            <p>Ahora que lo sabes, solo me queda preguntarte algo importante...</p>
            <p><strong>¿Quieres ser mi pareja?</strong></p>
            <a href="https://wa.me/36358604=Hola!%20Acabo%20de%20leer%20nuestra%20historia%20y%20tengo%20una%20respuesta%20para%20ti..." class="btn">Responder en WhatsApp</a>
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
