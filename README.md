<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>이지은 포트폴리오</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        @keyframes glitch {
            0% { text-shadow: 2px 2px #ff00ff, -2px -2px #00ffff; }
            50% { text-shadow: -2px -2px #ff00ff, 2px 2px #00ffff; }
            100% { text-shadow: 2px 2px #ff00ff, -2px -2px #00ffff; }
        }
        
        body {
            font-family: 'Arial', sans-serif;
            background-color: #0a0a0a;
            color: #00eaff;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        header {
            background: linear-gradient(90deg, #002244, #001122);
            padding: 20px;
        }
        h1 {
            font-size: 2em;
            color: #00eaff;
            animation: glitch 1s infinite alternate;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 15px;
        }
        nav ul li a {
            color: #00eaff;
            text-decoration: none;
            font-size: 1.2em;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #ff00ff;
            text-shadow: 0 0 5px #ff00ff;
        }
        section {
            padding: 50px 20px;
            border-bottom: 1px solid #00eaff;
            position: relative;
            overflow: hidden;
        }
        footer {
            background: #001122;
            padding: 20px;
            margin-top: 20px;
        }
        
        .neon-text {
            font-size: 1.5em;
            color: #00eaff;
            text-shadow: 0 0 5px #00eaff, 0 0 10px #00eaff;
        }
        
        @keyframes glow {
            0% { box-shadow: 0 0 5px #00eaff; }
            50% { box-shadow: 0 0 20px #00eaff; }
            100% { box-shadow: 0 0 5px #00eaff; }
        }
        .glow-button {
            background: #001122;
            color: #00eaff;
            padding: 10px 20px;
            border: 2px solid #00eaff;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s;
            animation: glow 1.5s infinite alternate;
        }
        .glow-button:hover {
            background: #00eaff;
            color: #001122;
        }
    </style>
</head>
<body>
    <header>
        <h1>이지은</h1>
        <nav>
            <ul>
                <li><a href="#home">홈</a></li>
                <li><a href="#portfolio">포트폴리오</a></li>
                <li><a href="#activity">활동 내역</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="home">
        <h2 class="neon-text">자기소개</h2>
        <p>안녕하세요! 저는 게임 개발을 사랑하는 이지은입니다.</p>
        <button class="glow-button">더 알아보기</button>
    </section>
    
    <section id="portfolio">
        <h2 class="neon-text">포트폴리오</h2>
        <p>여기에 프로젝트 목록을 추가할 수 있습니다.</p>
    </section>
    
    <section id="activity">
        <h2 class="neon-text">활동 내역</h2>
        <p>오파츠에서 진행한 활동들을 소개하는 공간입니다.</p>
    </section>
    
    <footer>
        <p>&copy; 2025 이지은. 모든 권리 보유.</p>
    </footer>
    
    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const button = document.querySelector(".glow-button");
            button.addEventListener("mouseover", () => {
                button.style.boxShadow = "0 0 20px #ff00ff";
            });
            button.addEventListener("mouseleave", () => {
                button.style.boxShadow = "0 0 5px #00eaff";
            });
        });
    </script>
</body>
</html>
