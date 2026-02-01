<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Ayush</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100-vh;
            background-color: #ffebee;
            font-family: 'Arial', sans-serif;
            text-align: center;
        }
        h1 { color: #d32f2f; }
        .buttons { margin-top: 20px; }
        button {
            padding: 15px 25px;
            font-size: 1.2rem;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        #yesBtn { background-color: #4caf50; color: white; margin-right: 10px; }
        #noBtn { background-color: #f44336; color: white; position: absolute; }
    </style>
</head>
<body>

    <div id="main-card">
        <h1 id="question">Ayush, will you be my Valentine? 💖</h1>
        <div class="buttons">
            <button id="yesBtn" onclick="celebrate()">Yes</button>
            <button id="noBtn" onmouseover="moveButton()">No</button>
        </div>
    </div>

    <script>
        function moveButton() {
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 100);
            const noBtn = document.getElementById('noBtn');
            noBtn.style.left = x + 'px';
            noBtn.style.top = y + 'px';
        }

        function celebrate() {
            document.getElementById('main-card').innerHTML = `
                <h1>YAY! ❤️</h1>
                <p>I knew you'd say yes!</p>
                <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHpueGZ4eGZ4eGZ4eGZ4eGZ4eGZ4eGZ4eGZ4eGZ4eGZ4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/c76IJLufpN61i/giphy.gif" width="300">
            `;
        }
    </script>
</body>
</html>
# For-Rasmalai-
