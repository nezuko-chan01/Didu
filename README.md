<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday 🎉💖</title>
    <!-- Google Fonts for cute style -->
    <link href="https://fonts.googleapis.com/css2?family=Patrick+Hand&family=Sacramento&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Patrick Hand', cursive;
            background: #fff0f5;
            color: #333;
        }

        /* Button Style */
        .popup-btn {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ffe0f0, #d0f0ff);
            font-size: 2rem;
            cursor: pointer;
            color: #ff69b4;
            font-weight: bold;
            transition: transform 0.2s;
        }

        .popup-btn:hover {
            transform: scale(1.1);
        }

        /* Popup Sticker */
        .popup {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: #fff0f5;
            border: 4px dashed #ff69b4;
            padding: 30px;
            text-align: center;
            z-index: 100;
            display: none;
            border-radius: 20px;
            box-shadow: 0 0 15px rgba(0,0,0,0.2);
            animation: bounce 0.5s;
        }

        @keyframes bounce {
            0% {transform: translate(-50%, -60%) scale(0.5);}
            100% {transform: translate(-50%, -50%) scale(1);}
        }

        .popup img {
            width: 150px;
            margin: 10px 0;
        }

        .popup h2 {
            color: #ff1493;
            font-family: 'Sacramento', cursive;
        }

        /* Birthday Note Section */
        .note-section {
            padding: 50px 20px;
            background: #fff0f5;
            text-align: center;
        }

        .note-section h1 {
            font-family: 'Sacramento', cursive;
            font-size: 3rem;
            color: #ff69b4;
            margin-bottom: 20px;
        }

        .note-section p {
            font-size: 1.5rem;
            max-width: 800px;
            margin: 0 auto;
            line-height: 2;
            color: #555;
        }

        .note-section img {
            width: 200px;
            margin: 20px;
        }

        /* Floating Sticker GIF */
        .floating-gif {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 120px;
            z-index: 50;
        }

    </style>
</head>
<body>

    <!-- Press here button -->
    <div class="popup-btn" id="openPopup">🎈 Press Here for a Surprise 🎈</div>

    <!-- Popup Sticker -->
    <div class="popup" id="popup">
        <h2>🎉 Happy Birthday! 🎉</h2>
        <img src="https://media.giphy.com/media/3o6Zt481isNVuQI1l6/giphy.gif" alt="Birthday Gif">
        <p>Wishing you lots of love, joy, and yummy cake! 🍰💖</p>
        <button onclick="closePopup()" style="padding:10px 20px; font-size:1rem; border:none; border-radius:10px; background:#ff69b4; color:white; cursor:pointer;">Close</button>
    </div>

    <!-- Birthday Note Section -->
    <div class="note-section">
        <h1>💌 A Special Birthday Note 💌</h1>
        <p>
            Hey there! On this beautiful day, I just want to tell you how amazing you are. 🌸  
            Your smile lights up the room, your heart spreads so much love, and your laughter makes every moment brighter.  
            May this year bring you endless happiness, sweet surprises, and dreams coming true. 🎂💖  

            Remember, life is a journey and birthdays are little milestones to celebrate your awesomeness!  
            Keep shining, keep dreaming, and keep being the wonderful YOU that everyone loves so much. 🌈💫  
        </p>
        <img src="https://media.giphy.com/media/26ufdipQqU2lhNA4g/giphy.gif" alt="Cute Birthday Gif">
        <p>
            Sending you the biggest hugs, tightest squeezes, and all the cake you can eat! 🎂🥰  
            Happy Birthday again! May your day be as pastel-perfect and magical as this website. 🌸💖
        </p>
    </div>

    <!-- Floating GIF Sticker -->
    <img src="https://media.giphy.com/media/l0MYt5jPR6QX5pnqM/giphy.gif" class="floating-gif" alt="Floating Birthday GIF">

    <script>
        const popup = document.getElementById("popup");
        const btn = document.getElementById("openPopup");

        btn.addEventListener("click", () => {
            popup.style.display = "block";
        });

        function closePopup() {
            popup.style.display = "none";
        }
    </script>

</body>
</html>
