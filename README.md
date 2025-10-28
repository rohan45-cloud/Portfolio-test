<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Rohan Sharma | Front-End Developer</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }
        
        body {
            background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
            color: #fff;
            overflow-x: hidden;
        }
        
        header {
            position: fixed;
            width: 100%;
            top: 0;
            left: 0;
            padding: 1.2rem 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
            z-index: 100;
        }
        
        .logo a {
            color: #00e8f8;
            text-decoration: none;
            font-size: 1.6rem;
            font-weight: 700;
        }
        
        nav a {
            color: #fff;
            text-decoration: none;
            margin-left: 25px;
            font-weight: 500;
            transition: 0.3s;
            position: relative;
        }
        
        nav a::after {
            content: '';
            width: 0;
            height: 2px;
            background: #00e8f8;
            position: absolute;
            bottom: -6px;
            left: 0;
            transition: 0.4s;
        }
        
        nav a:hover::after {
            width: 100%;
        }
        
        section {
            padding: 6rem 8%;
            min-height: 100vh;
        }
        /* HERO SECTION */
        
        .main {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            padding-top: 8rem;
            animation: fadeIn 1s ease-in;
        }
        
        .detail {
            max-width: 550px;
        }
        
        .detail h1 {
            font-size: 2.8rem;
            font-weight: 700;
            line-height: 1.3;
        }
        
        .detail h1 span {
            color: #00e8f8;
        }
        
        .detail p {
            color: #ccc;
            margin-top: 1.2rem;
            line-height: 1.7;
            font-size: 1.05rem;
        }
        
        .social {
            display: flex;
            gap: 1.2rem;
            margin-top: 2rem;
        }
        
        .social a {
            color: #00e8f8;
            border: 2px solid #00e8f8;
            border-radius: 50%;
            padding: 0.5rem;
            font-size: 1.2rem;
            width: 38px;
            text-align: center;
            transition: 0.3s;
        }
        
        .social a:hover {
            background: #00e8f8;
            color: #1f252e;
            box-shadow: 0 0 25px #00e8f8;
            transform: scale(1.1);
        }
        
        .images img {
            width: 360px;
            border-radius: 50%;
            border: 4px solid #00e8f8;
            box-shadow: 0 0 40px #00e8f8;
            transition: transform 0.4s;
        }
        
        .images img:hover {
            transform: scale(1.05) rotate(3deg);
        }
        /* ABOUT */
        
        .about {
            text-align: center;
            max-width: 750px;
            margin: auto;
        }
        
        .about p {
            color: #ccc;
            line-height: 1.7;
        }
        
        h2 {
            color: #00e8f8;
            margin-bottom: 1.5rem;
            font-size: 2rem;
            text-align: center;
        }
        /* SKILLS */
        
        .skills {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
            margin-top: 2rem;
        }
        
        .skill {
            text-align: center;
            background: rgba(255, 255, 255, 0.1);
            padding: 25px;
            border-radius: 12px;
            width: 130px;
            transition: 0.3s;
        }
        
        .skill img {
            width: 65px;
            margin-bottom: 10px;
        }
        
        .skill:hover {
            transform: translateY(-10px);
            box-shadow: 0 0 20px #00e8f8;
        }
        /* PROJECTS */
        
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 2rem;
        }
        
        .project-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 20px;
            transition: 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 0 20px #00e8f8;
        }
        
        .project-card img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }
        /* CONTACT */
        
        .contact ul {
            list-style: none;
            text-align: center;
            line-height: 2;
        }
        
        .contact a {
            color: #00e8f8;
            text-decoration: none;
        }
        
        footer {
            text-align: center;
            padding: 1.5rem;
            color: #aaa;
            background: rgba(0, 0, 0, 0.3);
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
        
        @media (max-width: 768px) {
            .main {
                flex-direction: column;
                text-align: center;
            }
            .images img {
                width: 280px;
                margin-top: 2rem;
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="logo"><a href="#home">Rohan.</a></div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="home" class="main">
        <div class="detail">
            <h1>Hi, I'm <span>Rohan Sharma</span></h1>
            <p>A passionate Front-End Developer skilled in crafting modern, responsive, and user-friendly websites using HTML, CSS, and JavaScript. I focus on clean design, smooth interactions, and performance.</p>
            <div class="social">
                <a href="#"><i class="bi bi-github"></i></a>
                <a href="#"><i class="bi bi-linkedin"></i></a>
                <a href="#"><i class="bi bi-instagram"></i></a>
                <a href="#"><i class="bi bi-facebook"></i></a>
            </div>
        </div>
        <div class="images">
            <img src="images/profile.jpg" alt="Rohan Sharma">
        </div>
    </section>

    <section id="about" class="about">
        <h2>About Me</h2>
        <p>I'm a Front-End Developer based in Greater Noida, Uttar Pradesh. I enjoy building beautiful, functional, and responsive websites using HTML, CSS, and JavaScript. My mission is to deliver exceptional digital experiences that are accessible and
            efficient across all devices.</p>
    </section>

    <section id="skills">
        <h2>Skills</h2>
        <div class="skills">
            <div class="skill"><img src="images/HTML5 (1).png" alt="HTML">
                <p>HTML</p>
            </div>
            <div class="skill"><img src="images/CSS3.png" alt="CSS">
                <p>CSS</p>
            </div>
            <div class="skill"><img src="images/JavaScript.png" alt="JavaScript">
                <p>JavaScript</p>
            </div>
        </div>
    </section>

    <section id="projects">
        <h2>Projects</h2>
        <div class="project-grid">
            <div class="project-card">
                <img src="images/wheather.jpeg" alt="Weather App">
                <h3>Weather App</h3>
                <p>An interactive weather app that fetches live data from the OpenWeather API and displays current temperature, humidity, and wind speed with a clean UI.</p>
            </div>
            <div class="project-card">
                <img src="images/music.png" alt="Music Player">
                <h3>Music Player</h3>
                <p>A fully functional music player with play, pause, next, and previous buttons, a progress bar, and album art built using HTML, CSS, and JS.</p>
            </div>
            <div class="project-card">
                <img src="images/gallery.jpg" alt="Image Gallery">
                <h3>Image Gallery</h3>
                <p>A responsive photo gallery featuring a fullscreen lightbox, hover animations, and grid layout optimized for all devices.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact</h2>
        <ul>
            <li>📞 Phone: +91 9129775531</li>
            <li>📧 Email: rohansharmaxyz45@gmail.com</li>
            <li>📍 Location: Greater Noida, Uttar Pradesh</li>
            <li>🔗 <a href="#">LinkedIn Profile</a></li>
        </ul>
    </section>

    <footer>
        <p>© 2025 Rohan Sharma | All Rights Reserved</p>
    </footer>
</body>

</html>
