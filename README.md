# argument-generator
argument-generator
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Argument Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        input[type="text"] {
            width: 60%;
            padding: 10px;
            font-size: 16px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin-top: 10px;
            cursor: pointer;
        }
        img {
            margin-top: 20px;
            max-width: 100%;
            height: auto;
        }
        .subtitle {
            margin-top: 10px;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <h1>Argument Generator</h1>
    <p>Type your statement and get a counter-argument!</p>
    <input type="text" id="userInput" placeholder="Enter your statement...">
    <br>
    <button onclick="generateArgument()">Submit</button>
    <div id="result">
        <img id="resultImage" src="" alt="Argument Image">
        <p class="subtitle" id="subtitle"></p>
    </div>

    <script>
        function generateArgument() {
            const userInput = document.getElementById('userInput').value;
            const imageSearchQuery = `funny disagreement meme ${userInput}`;

            // Use a free image from the web for simplicity
            const imageURL = `https://source.unsplash.com/featured/?${encodeURIComponent(imageSearchQuery)}`;
            
            document.getElementById('resultImage').src = imageURL;
            document.getElementById('subtitle').innerText = "ya! just like ur mamma’s ass";
        }
    </script>
</body>
</html>
