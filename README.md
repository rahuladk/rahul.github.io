<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffebf2;
        }
        .container {
            margin-top: 100px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .yes-btn {
            background-color: #ff4d6d;
            color: white;
        }
        .no-btn {
            background-color: #666;
            color: white;
        }
        .hidden {
            display: none;
        }
        img {
            width: 300px;
            border-radius: 10px;
            margin-top: 20px;
        }
        .message {
            font-size: 18px;
            margin-top: 20px;
            color: #d63384;
        }
    </style>
</head>
<body>

    <div class="container" id="question">
        <h1>Will you be my Valentine? ❤</h1>
        <button class="yes-btn" onclick="sayYes()">Yes</button>
        <button class="no-btn" onclick="askAgain()">No</button>
    </div>

    <div class="hidden" id="response">
        <h1>Yay! You said YES! 💖</h1>
        <img src="your-image.jpg" alt="Us together">
        <p class="message">
            My love, you are the most wonderful person in my life. You bring happiness and warmth into my world, and I can’t imagine my days without you. 
            You are kind, beautiful, and perfect in every way. I admire your smile, your heart, and the way you make every moment special.  
            Every day with you is a dream come true, and I promise to always cherish and love you.  
            Happy Valentine’s Day, my love! 💕
        </p>
        <audio controls autoplay>
            <source src="your-song.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
    </div>

    <script>
        function sayYes() {
            document.getElementById('question').classList.add('hidden');
            document.getElementById('response').classList.remove('hidden');
        }

        function askAgain() {
            alert("Think again! 💕");
        }
    </script>

</body>
</html>
