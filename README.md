<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eryk - Developer</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', sans-serif;
            background: linear-gradient(135deg, #0f172a, #020617);
            color: white;
            overflow-x: hidden;
        }

        .container {
            max-width: 1000px;
            margin: auto;
            padding: 40px 20px;
        }

        /* CARD */
        .card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 0 40px rgba(0,0,0,0.5);
            text-align: center;
            animation: fadeIn 1.2s ease;
        }

        h1 {
            font-size: 42px;
            margin-bottom: 10px;
        }

        .typing {
            color: #38bdf8;
            font-weight: bold;
        }

        p {
            color: #94a3b8;
            margin-bottom: 25px;
        }

        /* SOCIAL */
        .social a {
            display: inline-block;
            margin: 10px;
            padding: 10px 20px;
            border-radius: 30px;
            text-decoration: none;
            color: white;
            transition: 0.3s;
            font-weight: bold;
        }

        .x {
            background: black;
        }

        .fb {
            background: #1877f2;
        }

        .social a:hover {
            transform: scale(1.1);
            box-shadow: 0 0 15px rgba(255,255,255,0.3);
        }

        /* SKILLS */
        .skills {
            margin-top: 40px;
            text-align: left;
        }

        .skills h2 {
            margin-bottom: 20px;
        }

        .skill {
            margin-bottom: 15px;
        }

        .skill-name {
            margin-bottom: 5px;
        }

        .bar {
            height: 10px;
            background: #1e293b;
            border-radius: 10px;
            overflow: hidden;
        }

        .progress {
            height: 100%;
            background: linear-gradient(90deg, #38bdf8, #22c55e);
            animation: load 2s ease;
        }

        /* FOOTER */
        footer {
            text-align: center;
            margin-top: 40px;
            color: #64748b;
        }

        /* ANIMATION */
        @keyframes load {
            from { width: 0; }
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

    </style>
</head>
<body>

    <div class="container">
        <div class="card">

            <h1>Eryk 👋</h1>
            <p class="typing">Web Developer | C++ Learner | Tech Enthusiast</p>

            <p>
                Xin chào! Tôi là Eryk — một người đam mê lập trình và công nghệ. 
                Tôi đang học và phát triển kỹ năng trong lĩnh vực lập trình web và C++.
            </p>

            <div class="social">
                <a class="x" href="https://x.com/Erykle1blp" target="_blank">X</a>
                <a class="fb" href="https://www.facebook.com/anggkhoi.806438" target="_blank">Facebook</a>
            </div>

            <!-- SKILLS -->
            <div class="skills">
                <h2>💻 Kỹ năng</h2>

                <div class="skill">
                    <div class="skill-name">HTML</div>
                    <div class="bar"><div class="progress" style="width: 90%"></div></div>
                </div>

                <div class="skill">
                    <div class="skill-name">CSS</div>
                    <div class="bar"><div class="progress" style="width: 80%"></div></div>
                </div>

                <div class="skill">
                    <div class="skill-name">C++</div>
                    <div class="bar"><div class="progress" style="width: 70%"></div></div>
                </div>

                <div class="skill">
                    <div class="skill-name">JavaScript</div>
                    <div class="bar"><div class="progress" style="width: 60%"></div></div>
                </div>

            </div>

        </div>

        <footer>
            © 2026 Eryk. Made with ❤️
        </footer>
    </div>

</body>
</html>
