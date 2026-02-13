<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Valentine’s Day ❤️</title>
<style>
    body {
        margin: 0;
        padding: 0;
        background: linear-gradient(to top right, #ff9a9e, #fad0c4);
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: 'Arial', sans-serif;
        overflow: hidden;
    }

    .card {
        background: white;
        padding: 40px;
        border-radius: 20px;
        box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        text-align: center;
        animation: fadeIn 2s ease-in-out;
    }

    h1 {
        color: #ff4b5c;
        font-size: 2.5em;
        margin-bottom: 10px;
    }

    p {
        font-size: 1.2em;
        color: #444;
    }

    .heart {
        position: absolute;
        bottom: -50px;
        font-size: 24px;
        animation: floatUp 5s linear infinite;
        color: #ff4b5c;
    }

    @keyframes fadeIn {
        from {opacity: 0; transform: scale(0.8);}
        to {opacity: 1; transform: scale(1);}
    }

    @keyframes floatUp {
        0% {
            transform: translateY(0);
            opacity: 1;
        }
        100% {
            transform: translateY(-100vh);
            opacity: 0;
        }
    }
</style>
</head>
<body>

<div class="card">
    <h1>Happy Valentine’s Day ❤️</h1>
    <p>You make my world brighter every day.</p>
    <p>Will you be my Valentine? 💌</p>
</div>

<script>
    function createHeart() {
        const heart = document.createElement("div");
        heart.classList.add("heart");
        heart.innerHTML = "❤️";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.animationDuration = (Math.random() * 2 + 3) + "s";
        document.body.appendChild(heart);

        setTimeout(() => {
            heart.remove();
        }, 5000);
    }

    setInterval(createHeart, 300);
</script>

</body>
</html>
