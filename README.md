
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Someone Special ❤️</title>
<style>
    body {
        margin: 0;
        padding: 0;
        background: linear-gradient(135deg, #ff758c, #ff7eb3);
        font-family: 'Segoe UI', sans-serif;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        overflow: hidden;
        text-align: center;
        color: white;
    }

    .container {
        background: rgba(255, 255, 255, 0.15);
        padding: 40px;
        border-radius: 20px;
        backdrop-filter: blur(10px);
        width: 350px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        animation: fadeIn 1.5s ease-in-out;
    }

    h2 {
        margin-bottom: 20px;
    }

    button {
        padding: 10px 20px;
        margin: 8px;
        border: none;
        border-radius: 20px;
        background: white;
        color: #ff4b7d;
        font-weight: bold;
        cursor: pointer;
        transition: 0.3s;
    }

    button:hover {
        background: #ff4b7d;
        color: white;
        transform: scale(1.1);
    }

    .heart {
        position: absolute;
        bottom: -20px;
        font-size: 20px;
        animation: floatUp 6s linear infinite;
    }

    @keyframes floatUp {
        0% { transform: translateY(0); opacity: 1; }
        100% { transform: translateY(-100vh); opacity: 0; }
    }

    @keyframes fadeIn {
        from {opacity: 0; transform: scale(0.9);}
        to {opacity: 1; transform: scale(1);}
    }
</style>
</head>
<body>

<div class="container" id="box">
    <h2>Hi beautiful ❤️</h2>
    <p>How was your day?</p>
    <button onclick="nextQuestion(1)">Good 😊</button>
    <button onclick="nextQuestion(1)">Bad 😔</button>
</div>

<script>
    function nextQuestion(step) {
        const box = document.getElementById("box");

        if(step === 1) {
            box.innerHTML = `
                <h2>I hope it gets even better 💕</h2>
                <p>How are you feeling right now?</p>
                <button onclick="nextQuestion(2)">Happy 😄</button>
                <button onclick="nextQuestion(2)">Tired 😴</button>
                <button onclick="
