<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Eryk - Portfolio</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: 'Segoe UI', sans-serif;
    color: white;
    background: url("https://images.unsplash.com/photo-1507525428034-b723cf961d3e") no-repeat center/cover;
}

/* OVERLAY */
body::before {
    content: "";
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.6);
    z-index: -1;
}

/* NAV */
nav {
    position: fixed;
    width: 100%;
    top: 0;
    background: rgba(0,0,0,0.5);
    backdrop-filter: blur(10px);
    display: flex;
    justify-content: space-between;
    padding: 15px 40px;
    z-index: 1000;
}

nav h2 {
    color: #38bdf8;
}

nav a {
    color: white;
    margin-left: 20px;
    text-decoration: none;
    transition: 0.3s;
}

nav a:hover {
    color: #38bdf8;
}

/* HERO */
.hero {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.hero h1 {
    font-size: 55px;
}

.typing {
    color: #38bdf8;
    margin-top: 10px;
}

/* BUTTON */
.btn {
    margin-top: 20px;
    padding: 12px 25px;
    border-radius: 30px;
    background: #38bdf8;
    color: black;
    text-decoration: none;
    display: inline-block;
    transition: 0.3s;
}

.btn:hover {
    transform: scale(1.1);
}

/* SECTION */
.section {
    padding: 80px 20px;
    max-width: 1000px;
    margin: auto;
    animation: fadeUp 1s ease;
}

@keyframes fadeUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
}

/* CARD */
.card {
    background: rgba(255,255,255,0.1);
    padding: 20px;
    border-radius: 15px;
    margin: 10px 0;
    backdrop-filter: blur(10px);
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 0 20px rgba(56,189,248,0.5);
}

/* SKILLS */
.bar {
    height: 8px;
    background: #020617;
    border-radius: 10px;
}

.progress {
    height: 100%;
    background: #38bdf8;
}

/* CONTACT */
.contact {
    text-align: center;
}

/* SOCIAL */
.social a {
    margin: 10px;
    display: inline-block;
    padding: 10px 20px;
    border-radius: 20px;
    text-decoration: none;
    color: white;
    transition: 0.3s;
}

.social a:hover {
    transform: scale(1.1);
}

.x { background: black; }
.fb { background: #1877f2; }
.tiktok { background: #111; }

footer {
    text-align: center;
    padding: 20px;
    color: #cbd5f5;
}
</style>
</head>

<body>

<nav>
    <h2>Eryk</h2>
    <div>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
    </div>
</nav>

<section class="hero" id="home">
    <div>
        <h1>Hi, I'm Eryk 👋</h1>
        <div class="typing" id="typing"></div>
        <a href="#contact" class="btn">Liên hệ</a>
    </div>
</section>

<section class="section" id="about">
    <h2>👨‍💻 About Me</h2>
    <div class="card">Tôi là một người yêu thích lập trình và sáng tạo.</div>
    <div class="card">Tôi tập trung vào HTML, CSS và C++.</div>
    <div class="card">Luôn học hỏi và phát triển mỗi ngày.</div>
</section>

<section class="section" id="skills">
    <h2>💻 Skills</h2>

    HTML
    <div class="bar"><div class="progress" style="width:90%"></div></div>

    CSS
    <div class="bar"><div class="progress" style="width:85%"></div></div>

    C++
    <div class="bar"><div class="progress" style="width:70%"></div></div>
</section>

<section class="section" id="contact">
    <h2>📞 Contact</h2>
    <div class="contact">
        <p>Hotline: <b>0334478903</b></p>

        <div class="social">
            <a class="x" href="https://x.com/Erykle1blp" target="_blank">X</a>
            <a class="fb" href="https://www.facebook.com/anggkhoi.806438" target="_blank">Facebook</a>
            <a class="tiktok" href="https://www.tiktok.com/@dkou07" target="_blank">TikTok</a>
        </div>
    </div>
</section>

<footer>
    © 2026 Eryk - Portfolio
</footer>

<script>
const text = "Simple • Clean • Personal";
let i = 0;
function typing(){
    if(i < text.length){
        document.getElementById("typing").innerHTML += text.charAt(i);
        i++;
        setTimeout(typing, 50);
    }
}
typing();
</script>

</body>
</html>
