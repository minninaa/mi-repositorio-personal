<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>MIAU MIAU MIAU</title>
    <style>
        body {
            background-color: #fce4ec;
            font-family: 'Comic Sans MS', cursive;
            text-align: center;
            overflow-x: hidden;
        }
        .miau-flotante {
            position: fixed;
            color: #ff4081;
            font-weight: bold;
            z-index: -1;
            opacity: 0.6;
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            background: white;
            padding: 20px;
            border-radius: 30px;
            border: 5px dashed #ff4081;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        h1 { color: #d81b60; font-size: 3em; }
        .foto-gatito {
            width: 100%;
            border-radius: 20px;
            margin: 20px 0;
        }
        .boton-miau {
            background: #ff4081;
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            font-size: 1.5em;
            cursor: pointer;
            transition: transform 0.2s;
        }
        .boton-miau:hover { transform: scale(1.1) rotate(5deg); }
    </style>
</head>
<body>

    <div class="miau-flotante" style="top: 10%; left: 5%;">Miau?</div>
    <div class="miau-flotante" style="top: 20%; right: 10%;">¡MIAU!</div>
    <div class="miau-flotante" style="bottom: 15%; left: 15%;">miau miau</div>
    <div class="miau-flotante" style="top: 50%; left: 2%;">purr... miau</div>
    <div class="miau-flotante" style="bottom: 5%; right: 5%;">MIAU.</div>

    <div class="container">
        <h1>Miau Miau Miau Miau</h1>
        <p>Miau miau, miau miau miau. ¡Miau!</p>
        
        http://googleusercontent.com/image_generation_content/0

        <p>miau miau miau miau miau miau miau miau miau miau miau miau</p>
        
        <button class="boton-miau" onclick="alert('¡MIAAAU!')">Presiona para Miau</button>
        
        <div style="margin-top: 20px;">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHJndnZueXp3eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/3oriO0OEd9QIDdllqo/giphy.gif" width="100" alt="Gatito bailando">
        </div>
    </div>

    <script>
        // Generador automático de miaus al hacer clic en cualquier parte
        document.addEventListener('click', (e) => {
            const miau = document.createElement('div');
            miau.innerText = 'MIAU';
            miau.style.position = 'absolute';
            miau.style.left = e.pageX + 'px';
            miau.style.top = e.pageY + 'px';
            miau.style.color = '#ad1457';
            miau.style.pointerEvents = 'none';
            document.body.appendChild(miau);
            
            setTimeout(() => miau.remove(), 1000);
        });
    </script>
</body>
</html>
