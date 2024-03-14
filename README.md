<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Number Guessing Game</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
    }
    #result {
        font-size: 1.5em;
        margin-top: 20px;
    }
</style>
</head>
<body>
    <h1>Number Guessing Game</h1>
    <p>Guess a number between 1 and 10:</p>
    <input type="text" id="guessInput">
    <button onclick="checkGuess()">Submit Guess</button>
    <p id="result"></p>

    <script>
        let secretNumber = Math.floor(Math.random() * 10) + 1;
        let attempts = 0;

        function checkGuess() {
            let guess = parseInt(document.getElementById('guessInput').value);
            attempts++;

            if (guess === secretNumber) {
                document.getElementById('result').innerHTML = `Congratulations! You guessed the number in ${attempts} attempts.`;
            } else if (guess < secretNumber) {
                document.getElementById('result').innerHTML = 'Try a higher number.';
            } else {
                document.getElementById('result').innerHTML = 'Try a lower number.';
            }
        }
    </script>
</body>
</html>
- 👋 Hi, I’m @majid2000012
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
majid2000012/majid2000012 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
