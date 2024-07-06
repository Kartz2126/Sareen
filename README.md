![image](https://github.com/Kartz2126/Sareen/assets/174878664/2bcd2386-a5cd-431e-a686-d7921588c741)<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tommy Question</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <div class="container">
        <p>Can you send me a photo of Tommy?</p>
        <button id="yesButton">Yes</button>
        <button id="noButton">No</button>
    </div>
    <script>
        const yesButton = document.getElementById('yesButton');
        const noButton = document.getElementById('noButton');
        const catGifUrl = 'https://media1.giphy.com/media/rBszdmXbzglQUX7N4j/giphy.gif?cid=6c09b952r8ksdljicnf2jrlzsbjyn26ak00r9tavhiaipcea&ep=v1_internal_gif_by_id&rid=giphy.gif&ct=g';

        const noButtonTexts = [
            'Adichi saavedichiruve',
            'I miss Tommy',
            'Pleaseeee',
            'Cut panniruve',
            'Ungaluku vere vali iruku nenekiringelaa?',
            'Ungalukella manasatchiye illeya?',
            'Kalnenjakaare',
            'Yes'
        ];

        yesButton.addEventListener('click', () => {
            window.location.href = catGifUrl;
        });

        let noClickCount = 0;
        noButton.addEventListener('click', () => {
            if (noClickCount < noButtonTexts.length) {
                noButton.textContent = noButtonTexts[noClickCount];
                noClickCount++;
            }
            if (noClickCount === noButtonTexts.length) {
                yesButton.style.display = 'inline';
            }
        });
    </script>
</body>
</html>
