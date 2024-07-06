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
        }
        .container {
            text-align: center;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .button {
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            background-color: #007bff;
            color: white;
            cursor: pointer;
            font-size: 16px;
        }
        .button:hover {
            background-color: #0056b3;
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
        document.getElementById('yesButton').onclick = function() {
            window.location.href = 'https://giphy.com/gifs/rBszdmXbzglQUX7N4j';
        };

        let noButton = document.getElementById('noButton');
        noButton.onclick = function() {
            noButton.innerText = 'Adichi saavedichiruve';
            noButton.onclick = function() {
                noButton.innerText = 'I miss Tommy';
                noButton.onclick = function() {
                    noButton.innerText = 'Pleaseeee';
                    noButton.onclick = function() {
                        noButton.innerText = 'Cut panniruve';
                        noButton.onclick = function() {
                            noButton.innerText = 'Ungaluku vere vali iruku nenekiringelaa?';
                            noButton.onclick = function() {
                                noButton.innerText = 'Ungalukella manasatchiye illeya?';
                                noButton.onclick = function() {
                                    noButton.innerText = 'Kalnenjakaare';
                                    noButton.onclick = function() {
                                        noButton.innerText = 'Yes';
                                        noButton.onclick = function() {
                                            window.location.href = 'https://giphy.com/gifs/rBszdmXbzglQUX7N4j';
                                        };
                                    };
                                };
                            };
                        };
                    };
                };
            };
        };
    </script>
</body>
</html>
