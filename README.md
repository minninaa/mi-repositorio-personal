# mi-repositorio-personal

# Meme Sound Buttons Page

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meme Sound Buttons</title>
    <style>
        body {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            font-family: Arial, sans-serif;
        }
        button {
            margin: 10px;
            padding: 15px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            background-color: #4CAF50;
            color: white;
        }
    </style>
</head>
<body>

  <button onclick="playSound('sound1.mp3')">Meme Sound 1</button>
  <button onclick="playSound('sound2.mp3')">Meme Sound 2</button>
  <button onclick="playSound('sound3.mp3')">Meme Sound 3</button>
  <button onclick="playSound('sound4.mp3')">Meme Sound 4</button>
  <button onclick="playSound('sound5.mp3')">Meme Sound 5</button>
  <button onclick="playSound('sound6.mp3')">Meme Sound 6</button>
  <button onclick="playSound('sound7.mp3')">Meme Sound 7</button>
  <button onclick="playSound('sound8.mp3')">Meme Sound 8</button>

  <audio id="audio" src=""></audio>

  <script>
        function playSound(sound) {
            const audio = document.getElementById('audio');
          audio.src = sound;
          audio.play();
       }
  </script>

</body>
</html>
