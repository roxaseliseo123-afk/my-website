[profile.indeec.html](https://github.com/user-attachments/files/26780231/profile.indeec.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Personal Profile</title>
    <style>
        /* ============================================
           PERSONAL PROFILE WEBSITE - EMBEDDED STYLES
           Modern Design with 2024 Color Trends
           ============================================ */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #1A1A2E;
            color: #ECF0F1;
            line-height: 1.6;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* HEADER */
        #main-header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 60px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
            border-bottom: 4px solid #FF6B6B;
        }

        #main-header h1 {
            font-family: Georgia, 'Times New Roman', serif;
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            letter-spacing: 2px;
        }

        .tagline {
            font-size: 1.3rem;
            font-weight: 300;
            opacity: 0.95;
            font-style: italic;
        }

        /* NAVIGATION */
        .navbar {
            background-color: rgba(45, 27, 78, 0.95);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .navbar ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }

        .navbar a {
            color: #ECF0F1;
            text-decoration: none;
            font-weight: 500;
            padding: 8px 16px;
            border-radius: 8px;
            transition: all 0.3s ease;
            position: relative;
        }

        .navbar a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, #FF6B6B, #FF8E53);
            transition: all 0.3s ease;
            transform: translateX(-50%);
        }

        .navbar a:hover {
            color: #FF6B6B;
            transform: translateY(-2px);
        }

        .navbar a:hover::after {
            width: 80%;
        }

        /* CONTENT SECTIONS */
        .content-section {
            background-color: rgba(255, 255, 255, 0.03);
            margin: 30px 0;
            padding: 40px;
            border-radius: 24px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .content-section:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2), 0 0 30px rgba(102, 126, 234, 0.3);
        }

        .content-section h2 {
            font-family: Georgia, 'Times New Roman', serif;
            font-size: 2.2rem;
            color: #9B7ED9;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid transparent;
            border-image: linear-gradient(90deg, #FF6B6B, #FF8E53);
            border-image-slice: 1;
            display: inline-block;
        }

        /* ABOUT SECTION */
        .about-content {
            display: grid;
            grid-template-columns: auto 1fr;
            gap: 40px;
            align-items: center;
        }

        .profile-image-container {
            position: relative;
        }

        .profile-image {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid transparent;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            padding: 5px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            transition: all 0.4s ease;
        }

        .profile-image:hover {
            transform: scale(1.05) rotate(3deg);
            box-shadow: 0 0 40px rgba(255, 107, 107, 0.4);
        }

        .about-text p {
            margin-bottom: 15px;
            font-size: 1.1rem;
            text-align: justify;
        }

        /* SKILLS */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .skill-card {
            background: linear-gradient(145deg, rgba(91, 46, 145, 0.3), rgba(45, 27, 78, 0.5));
            padding: 25px;
            border-radius: 16px;
            border: 1px solid rgba(155, 126, 217, 0.3);
            transition: all 0.3s ease;
        }

        .skill-card:hover {
            transform: translateY(-8px);
            border-color: #FF6B6B;
            box-shadow: 0 10px 30px rgba(255, 107, 107, 0.2);
        }

        .skill-card h3 {
            color: #FF8E53;
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .skill-card p {
            color: #7F8C8D;
            font-size: 0.95rem;
        }

        /* PROJECTS */
        .projects-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 20px;
        }

        .project-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 16px;
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.4s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            border-color: #9B7ED9;
        }

        .project-image {
            height: 200px;
            width: 100%;
        }

        .project-card h3 {
            padding: 15px 20px 0;
            color: #9B7ED9;
        }

        .project-card p {
            padding: 0 20px;
            color: #7F8C8D;
            margin-bottom: 15px;
        }

        .project-link {
            display: inline-block;
            margin: 0 20px 20px;
            color: #FF6B6B;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        .project-link:hover {
            color: #FF8E53;
        }

        /* CONTACT */
        .contact-info {
            text-align: center;
            padding: 20px;
        }

        .contact-info p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            color: #7F8C8D;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .contact-link {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 12px 24px;
            background: rgba(255, 255, 255, 0.1);
            border: 2px solid #9B7ED9;
            border-radius: 8px;
            color: #ECF0F1;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }

        .contact-link:hover {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-color: #FF6B6B;
            transform: translateY(-3px);
        }

        /* FOOTER */
        #main-footer {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            padding: 30px 0;
            margin-top: 50px;
            border-top: 3px solid #5B2E91;
            text-align: center;
        }

        #main-footer p {
            color: #7F8C8D;
            margin-bottom: 10px;
        }

        .footer-links a {
            color: #9B7ED9;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: #FF6B6B;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            #main-header h1 { font-size: 2.5rem; }
            .about-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
            .profile-image {
                width: 200px;
                height: 200px;
                margin: 0 auto;
            }
            .navbar ul { gap: 20px; }
            .content-section { padding: 25px; }
        }

        html { scroll-behavior: smooth; }
    </style>
</head>
<body>
    <header id="main-header">
        <div class="container">
            <h1>Alex Morgan</h1>
            <p class="tagline">Creative Developer & Digital Designer</p>
        </div>
    </header>

    <nav class="navbar">
        <div class="container">
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <main class="container">
        <section id="about" class="content-section">
            <h2>About Me</h2>
            <div class="about-content">
                <div class="profile-image-container">
                <img src="myphoto.jpg.jpg" alt="My Profile Photo" class="profile-image">
                </div>
                <div class="about-text">
                    <p>Hello! "I am a web developer driven by the challenge of bridging the gap between complex software issues and seamless user experiences. My passion lies in technical troubleshooting identifying 'external' bottlenecks and fixing them through clean, efficient code. I am currently honing my skills in modern web technologies with a singular goal: to build high performing digital solutions that solve real-world problems for businesses and individuals alike.".</p>
                    
                </div>
            </div>
        </section>

        <section id="skills" class="content-section">
            <h2>Skills & Expertise</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <h3>Basic HTML and CCS</h3>
                    <p>I want to learn more about HTML and CSS</p>
                </div>
                <div class="skill-card">
                    <h3>Bsic HardWare Troubleshooting</h3>
                    <p>a systematic, logical approach to diagnosing and resolving malfunctions in systems, software, or hardware</p>
                </div>
                <div class="skill-card">
                    <h3>Game Error fixer</h3>
                    <p>I Fix Other Games With External Problem</p>
                </div>                       
             </div>
        </section>

        <section id="projects" class="content-section">
            <h2>Featured Projects</h2>
            <div class="projects-container">
                <article class="project-card">
                    <div class="project-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);"></div>
                    <h3>E-Commerce Dashboard</h3>
                    <p>A responsive admin dashboard with data visualization and real-time analytics.</p>
                    <a href="#" class="project-link">View Project →</a>
                </article>
                <article class="project-card">
                    <div class="project-image" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);"></div>
                    <h3>Weather App</h3>
                    <p>Location-based weather application with 7-day forecasts and interactive maps.</p>
                    <a href="#" class="project-link">View Project →</a>
                </article>
                <article class="project-card">
                    <div class="project-image" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);"></div>
                    <h3>Task Manager</h3>
                    <p>Productivity app with drag-and-drop functionality and team collaboration features.</p>
                    <a href="#" class="project-link">View Project →</a>
                </article>
            </div>
        </section>

        <section id="contact" class="content-section">
            <h2>Get In Touch</h2>
            <div class="contact-info">
                <p>I'm always interested in hearing about new projects and opportunities.</p>
                <div class="social-links">
                    <a href="mailto:alex@example.com" class="contact-link">📧 Email Me</a>
                    <a href="https://linkedin.com" target="_blank" class="contact-link">💼 LinkedIn</a>
                    <a href="https://github.com" target="_blank" class="contact-link">🐙 GitHub</a>
                    <a href="https://twitter.com" target="_blank" class="contact-link">🐦 Twitter</a>
                </div>
            </div>
        </section>
    </main>

    <footer id="main-footer">
        <div class="container">
            <p>&copy; 2024 Alex Morgan. Crafted with 💜 and lots of ☕</p>
            <p class="footer-links">
                <a href="#">Privacy Policy</a> | 
                <a href="#">Terms of Use</a>
            </p>
        </div>
    </footer>
</body>
</html>
