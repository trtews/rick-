# rick-
<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>sranda.com</title>
    <style>
        body {
            background: linear-gradient(to right, #ffccff, #ccffcc);
            font-family: 'Comic Sans MS', cursive, sans-serif;
            text-align: center;
            overflow: hidden;
        }
        h1 {
            font-size: 3em;
            color: #ff3399;
            text-shadow: 2px 2px #ffffff;
            margin-top: 50px;
        }
        p {
            font-size: 1.5em;
            color: #333;
        }
        button {
            font-size: 1.5em;
            padding: 15px 30px;
            margin-top: 30px;
            background-color: #00ccff;
            border: 3px solid #0099cc;
            border-radius: 10px;
            cursor: pointer;
            transition: transform 0.2s;
        }
        button:hover {
            transform: scale(1.1);
        }
        .boty {
            position: absolute;
            font-size: 2em;
            pointer-events: none;
            animation: padani 5s linear infinite;
        }
        @keyframes padani {
            0% { top: -50px; }
            100% { top: 100vh; }
        }
    </style>
</head>
<body>
    <h1>Vítejte na sranda.com! 😄</h1>
    <p>Chceš V-Bucks zdarma? Klikni dole!</p>
    <button onclick="rickRoll()">V-Bucks zdarma! 💎</button>

    <script>
        function rickRoll() {
            window.location.href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ";
        }

        // Generování padajících bot
        function vytvorBotu() {
            const boty = document.createElement('div');
            boty.className = 'boty';
            boty.innerText = '👢';
            boty.style.left = Math.random() * window.innerWidth + 'px';
            boty.style.animationDuration = (3 + Math.random() * 4) + 's';
            document.body.appendChild(boty);

            setTimeout(() => boty.remove(), 7000);
        }

        setInterval(vytvorBotu, 300);
    </script>
</body>
</html>
