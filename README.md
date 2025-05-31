<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Profesional</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            font-family: 'Arial', sans-serif;
            color: white;
            overflow-x: hidden;
        }
        
        .bg-image {
            background-image: url('https://th.bing.com/th/id/R.17692021f84f98b019eae248407852aa?rik=k1cszLGMknhl5g&pid=ImgRaw&r=0');
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            height: 100%;
            filter: brightness(0.7);
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            z-index: -1;
        }
        
        .content {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100%;
            text-align: center;
            padding: 0 20px;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 30px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
        }
        
        .btn {
            background-color: #2b2727;
            border: none;
            color: white;
            padding: 15px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 1.2rem;
            margin: 20px 0;
            cursor: pointer;
            border-radius: 5px;
            transition: all 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .btn:hover {
            background-color: #181a19;
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }
        
        .hidden-text {
            display: none;
            background-color: rgba(0, 0, 0, 0.7);
            padding: 30px;
            border-radius: 10px;
            max-width: 600px;
            margin-top: 30px;
            animation: fadeIn 0.5s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="bg-image"></div>
    
    <div class="content">
        <h1>Hoc Tibi Est, David</h1>
        <button class="btn" onclick="mostrarTexto()">Ver mas..</button>
        
        <div id="textoOculto" class="hidden-text">
            <!-- Aquí puedes personalizar el texto que aparecerá -->
            <h2></h2>
            <p>
    
¡Oh, el hombre de oro! ¡Oh, el hombre fuerte!
domador de potros, vencedor de la suerte,
que tiene el vigor de Hércules o de Aquiles,
y en los ojos la luz de los astros gentiles.

Su brazo es el brazo que rige la historia,
su frente es la sede del sueño y la gloria,
y en su pecho, cual roca, se estrella el destino,
mientras ríe con risa de mar o de trino.

Es el héroe antiguo, es el nuevo titán,
el que pasa y se siente seguir por su afán,
el que lleva en el puño la espada o el libro,
y en el alma el divino fulgor del equilibrio.</p>
            <p>(Autor, Rubén Darío)</p>
        </div>
    </div>
    
    <script>
        function mostrarTexto() {
            const texto = document.getElementById('textoOculto');
            const boton = document.querySelector('.btn');
            
            if (texto.style.display === 'block') {
                texto.style.display = 'none';
                boton.textContent = 'VER MÁS';
            } else {
                texto.style.display = 'block';
                boton.textContent = 'OCULTAR';
            }
        }
    </script>
</body>
</html># David
