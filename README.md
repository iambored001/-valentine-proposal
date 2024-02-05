# -valentine-proposal
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Proposal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f5f5f5;
        }
        #container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
            margin-bottom: 20px;
        }
        button {
            font-size: 16px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            color: #ffffff;
        }
        #yes {
            background-color: #4CAF50;
        }
        #no {
            background-color: #f44336;
        }
    </style>
</head>
<body>
    <div id="container">
        <h1>Will You Be My Valentine?</h1>
        <img src='qiBXjgjgT.jpg' alt="Your romantic image">
        <p>Dear kaijomellowmarshbloonjaancutiepie,</p>
        <p>I've been thinking about you a lot, and I was wondering if you would be my Valentine. I would love to spend Valentine's Day with you and make it special.</p>
        <p>Please let me know what you think.</p>
        <button id="yes" onclick="showSweetMessage()">Yes</button>
        <button id="no" onclick="showNoMessage()">No</button>
    </div>

    <script>
        var attempts = 5;

        function showSweetMessage() {
            document.getElementById("container").innerHTML = `
                <h1>Thank You!</h1>
                <p>Dear kaijomellowmarshbloonjaancutiepie,</p>
                <p>I'm thrilled that you said yes! I can't wait to make Valentine's Day special with you.</p>
                <p>Sincerely,<br>your taha</p>
            `;
        }

        function showNoMessage() {
            if (attempts > 0) {
                var desperateMessages = [
                    "I think you misclicked, so click the correct option.",
                    "I think your mouse might be broken cause it is not clicking the right thing",
                    "WTF IS WRONG WITH YOU BITCH JUST CLICK YES",
                    "HUHHHH you really clicking no",
                    "I can't help but feel a bit heartbroken. Wishing you a wonderful Valentine's Day. Fucking bitch, you don't deserve anything in life. You are a stupid little human who looks like a mango which has been stepped on a million times and then pooped on."
                ];

                document.getElementById("container").innerHTML += `
                    <p>${desperateMessages[5 - attempts]}</p>
                    <p>Attempts left: ${attempts}</p>
                `;
                attempts--;
            } else {
                document.getElementById("container").innerHTML = `
                    <h1>Thank You!</h1>
                    <p>Dear kaijomellowmarshbloonjaancutiepie,</p>
                    <p>ohh you just wait you low peasent, i will ruin your entire generation you donkey ass human, just you wait</p>
                    <p>Sincerely,<br>your taha</p>
                `;
            }
        }
    </script>
</body>
</html>
