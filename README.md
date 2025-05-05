<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Change Background on Image Click</title>
    <style>
        body {
            text-align: center;
            padding: 50px;
            transition: background-color 0.5s ease;
        }
        button {
            cursor: pointer;
            width: 200px;
        }
    </style>
</head>
<body>

    <button alt="Click Me!" onclick="changeBackground()">click me</button>

    <script>
        function changeBackground() {
            const colors = ["#f4a261", "#2a9d8f", "#264653", "#e76f51", "#9b5de5"];
            document.body.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
        }
    </script>

</body>
</html>
