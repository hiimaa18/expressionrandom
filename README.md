# expressionrandom
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Absurd Compliment Generator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Absurd Compliment Generator</h1>
        <p id="compliment">Press the button to get a compliment!</p>
        <button id="generate">Generate Compliment</button>
    </div>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f0f8ff;
    text-align: center;
    padding: 50px;
}

.container {
    border: 2px solid #4a90e2;
    padding: 20px;
    border-radius: 10px;
    background-color: #ffffff;
}

button {
    padding: 10px 20px;
    background-color: #4a90e2;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #357ab8;
}
const compliments = [
    "You're like a cloud made of marshmallows!",
    "If you were a vegetable, you'd be a cute-cumber!",
    "Your smile is like a thousand fireworks in a pickle jar!",
    "You're as delightful as a unicorn in a tutu!",
    "If laughter were a currency, you'd be a millionaire!",
    "You have the grace of a gazelle on roller skates!",
    "You're the reason even the stars get jealous!",
    "Your hair looks like a majestic lion's mane!",
    "You must have a superpower because you brighten every room!",
    "You're as charming as a potato wearing sunglasses!"
];

document.getElementById("generate").addEventListener("click", () => {
    const randomIndex = Math.floor(Math.random() * compliments.length);
    document.getElementById("compliment").innerText = compliments[randomIndex];
});


