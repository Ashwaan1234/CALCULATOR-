<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="calculator">
        <input type="text" id="display" disabled>

        <div class="buttons">
            <button onclick="clearDisplay()">C</button>
            <button onclick="appendValue('/')">/</button>
            <button onclick="appendValue('*')">*</button>
            <button onclick="deleteLast()">DEL</button>

            <button onclick="appendValue('7')">7</button>
            <button onclick="appendValue('8')">8</button>
            <button onclick="appendValue('9')">9</button>
            <button onclick="appendValue('-')">-</button>

            <button onclick="appendValue('4')">4</button>
            <button onclick="appendValue('5')">5</button>
            <button onclick="appendValue('6')">6</button>
            <button onclick="appendValue('+')">+</button>

            <button onclick="appendValue('1')">1</button>
            <button onclick="appendValue('2')">2</button>
            <button onclick="appendValue('3')">3</button>
            <button onclick="calculate()">=</button>

            <button onclick="appendValue('0')" class="zero">0</button>
            <button onclick="appendValue('.')">.</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
body {
    background-color: #f0f4f8;
    font-family: 'Segoe UI', sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.calculator {
    background-color: #fff;
    padding: 20px;
    border-radius: 15px;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
}

#display {
    width: 100%;
    height: 60px;
    font-size: 2rem;
    margin-bottom: 20px;
    text-align: right;
    padding: 10px;
    border: 2px solid #ccc;
    border-radius: 10px;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 60px);
    grid-gap: 10px;
    justify-content: center;
}

button {
    height: 60px;
    font-size: 1.5rem;
    border: none;
    background-color: #004aad;
    color: white;
    border-radius: 10px;
    cursor: pointer;
}

button:hover {
    background-color: #003080;
}

.zero {
    grid-column: span 2;
}
calculator/
├── index.html
├── style.css
└── script.js
