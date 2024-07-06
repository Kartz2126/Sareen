<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tommy Question</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
            padding: 10px;
            box-sizing: border-box;
        }
        .container {
            text-align: center;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
            box-sizing: border-box;
        }
        .button {
            padding: 10px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            background-color: #007bff;
            color: white;
            cursor: pointer;
            font-size: 16px;
            width: 100%;
            box-sizing: border-box;
            transition: all 0.3s;
        }
        .button:hover {
            background-color: #0056b3;
        }
        h1 {
            font-size: 18px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Can you send me a photo of Tommy?</h1>
        <button class="button" id="yesButton">Yes</button>
        <button class="button" id="noButton">No</button>
    </div>
    <script>
        let yesButton = document.getElementById('yesButton');
        let noButton = document.getElementById('noButton');
        let noClickCount = 0;
        
        yesButton.onclick = function() {
            window.location.href = 'https://giphy.com/gifs/rBszdmXbzglQUX7N4j';
        };

        noButton.onclick = function() {
            noClickCount++;
            yesButton.style.fontSize = (16 + noClickCount * 4) + 'px';
            switch (noClickCount) {
                case 1:
                    noButton.innerText = 'Adichi saavedichiruve';
                    break;
                case 2:
                    noButton.innerText = 'I miss Tommy';
                    break;
                case 3:
                    noButton.innerText = 'Pleaseeee';
                    break;
                case 4:
                    noButton.innerText = 'Cut panniruve';
                    break;
                case 5:
                    noButton.innerText = 'Ungaluku vere vali iruku nenekiringelaa?';
                    break;
                case 6:
                    noButton.innerText = 'Ungalukella manasatchiye illeya?';
                    break;
                case 7:
                    noButton.innerText = 'Kalnenjakaare';
                    break;
                case 8:
                    noButton.innerText = 'Yes';
                    noButton.onclick = yesButton.onclick;
                    break;
                default:
                    break;
            }
        };
    </script>
</body>
</html>
