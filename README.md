<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Número Aleatorio</title>
    <style>
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
        }

        .number-display {
            font-size: 5rem;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="number-display" id="numberDisplay">Haz clic en cualquier lugar</div>

    <script>
        document.body.addEventListener("click", () => {
            const randomNumber = Math.floor(Math.random() * 100) + 1;
            document.getElementById("numberDisplay").textContent = randomNumber;
        });
    </script>
</body>
</html>
