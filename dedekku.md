<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Untuk Kamu</title>
    <style>
        /* Pengaturan dasar halaman */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(120deg, #ff9a9e, #fad0c4);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }

        .container {
            text-align: center;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.2);
            animation: fadeIn 2s ease-in-out;
        }

        h1 {
            font-size: 36px;
            color: #ff6f61;
            margin-bottom: 10px;
        }

        p {
            font-size: 18px;
            color: #555;
            margin: 10px 0;
            line-height: 1.5;
        }

        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 18px;
            color: #fff;
            background: #ff6f61;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.2s ease;
        }

        button:hover {
            transform: scale(1.1);
        }

        button:active {
            transform: scale(1);
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.8); }
            to { opacity: 1; transform: scale(1); }
        }

        /* Animasi balon */
        .balloon {
            position: absolute;
            width: 50px;
            height: 70px;
            background: #ff6f61;
            border-radius: 50% 50% 50% 50%;
            animation: float 5s infinite ease-in-out;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .balloon:nth-child(1) {
            left: 20%;
            animation-delay: 0s;
        }

        .balloon:nth-child(2) {
            left: 50%;
            animation-delay: 2s;
        }

        .balloon:nth-child(3) {
            left: 80%;
            animation-delay: 4s;
        }

        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-50px); }
            100% { transform: translateY(0); }
        }
    </style>
</head>
<body>
    <!-- Balon animasi -->
    <div class="balloon"></div>
    <div class="balloon"></div>
    <div class="balloon"></div>

    <!-- Kontainer konten -->
    <div class="container">
        <h1>Hei Kamu!</h1>
        <p>Aku cuma mau bilang, jangan terlalu khawatir ya. Aku selalu ada di sini, kok.</p>
        <p>Ingat, kita butuh saling percaya untuk membuat semuanya indah. Kamu luar biasa!</p>
        <button onclick="showLove()">Klik untuk Kejutan</button>
    </div>

    <script>
        function showLove() {
            alert("Aku sayang kamu! ❤️");
        }
    </script>
</body>
</html>
