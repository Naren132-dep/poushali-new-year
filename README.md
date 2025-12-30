# poushali-new-year
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy New Year Poushali 💖</title>
<style>
body {
    margin: 0;
    font-family: 'Comic Sans MS', cursive;
    background: radial-gradient(circle, #ff9a9e, #fad0c4);
    color: white;
    text-align: center;
    overflow: hidden;
}
h1 {
    font-size: 3em;
    margin-top: 60px;
    animation: glow 1.5s infinite alternate;
}
@keyframes glow {
    from { text-shadow: 0 0 10px #fff; }
    to { text-shadow: 0 0 30px #ff4d6d; }
}
.box {
    background: rgba(0,0,0,0.3);
    padding: 25px;
    border-radius: 20px;
    width: 80%;
    margin: auto;
    font-size: 1.2em;
}
.heart {
    position: absolute;
    animation: float 6s infinite;
    font-size: 25px;
}
@keyframes float {
    0% { transform: translateY(100vh); opacity: 0; }
    50% { opacity: 1; }
    100% { transform: translateY(-10vh); opacity: 0; }
}
#countdown {
    font-size: 1.5em;
    margin-top: 20px;
}
</style>
</head>
<body>

<h1>🎆 Happy New Year Poushali 💖</h1>

<div class="box">
💃 Hey Poushali! 🥰<br><br>

New Year resolution idea 💡  
👉 Smile more (because it looks cute on you 😌)  
👉 Laugh louder (bonus points if it’s at my jokes 🤭)  
👉 Stay amazing (non-negotiable 💖)<br><br>

If cuteness was currency,  
you’d already be a billionaire 💸😍<br><br>

May this year bring you  
✨ happiness  
✨ success  
✨ love  
✨ and someone who sends you silly links like this 😜💞
</div>

<div id="countdown"></div>

<script>
// Countdown
const newYear = new Date("Jan 1, 2026 00:00:00").getTime();
setInterval(() => {
    const now = new Date().getTime();
    const diff = newYear - now;
    if (diff > 0) {
        const d = Math.floor(diff / (1000*60*60*24));
        const h = Math.floor((diff % (1000*60*60*24)) / (1000*60*60));
        const m = Math.floor((diff % (1000*60*60)) / (1000*60));
        const s = Math.floor((diff % (1000*60)) / 1000);
        document.getElementById("countdown").innerHTML =
        `⏳ New Year arrives in ${d}d ${h}h ${m}m ${s}s 💕`;
    }
}, 1000);

// Floating hearts
setInterval(() => {
    const heart = document.createElement("div");
    heart.className = "heart";
    heart.innerHTML = "💖";
    heart.style.left = Math.random() * 100 + "vw";
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 6000);
}, 300);
</script>

</body>
</html>
