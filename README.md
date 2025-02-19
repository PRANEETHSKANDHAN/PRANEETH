<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PRANEETH SKANDHAN S - Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <script src="myportfolio.js"></script>
    <style>
        body{
            background-repeat: no-repeat;
            background-attachment: fixed;
        }
      /* Reset and base styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    color: #040404;
}

/* .background-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    z-index: -1;
    overflow: hidden;
} */
.background-container {
    position: fixed; /* Stays in place during scroll */
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1; /* Places the GIF behind other content */
    overflow: hidden; /* Prevents GIF from overflowing */
}

.background-container img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Ensures GIF covers the entire background */
}

#bgVideo {
    position: absolute;
    top: 50%;
    left: 50%;
    min-width: 100%;
    min-height: 100%;
    width: auto;
    height: auto;
    transform: translateX(-50%) translateY(-50%);
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header styles */
header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    backdrop-filter: blur(5px);
    z-index: 1000;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style-type: none;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    display: inline-block;
    padding: 15px 10px;
    color: #ffffff;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}

nav ul li a:hover {
    color: #3498db;
}

/* Section styles */
section {
    padding: 100px 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

h1, h2, h3 {
    margin-bottom: 20px;
}

h1 {
    font-size: 3rem;
}

h2 {
    font-size: 2.5rem;
    text-align: center;
}

/* Home section styles */
#home {
    text-align: center;
}

.profile-image {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    border: 4px solid #d47535;
    margin-bottom: 20px;
}

.cta-button {
    display: inline-block;
    background-color: #f17039;
    color: #ffffff;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s ease;
}

.cta-button:hover {
    background-color: #e67c31;
}

/* Skills section styles */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 20px;
    margin-top: 40px;
}

.skill-item {
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 10px;
    padding: 20px;
    text-align: center;
    transition: transform 0.3s ease;
}

.skill-item:hover {
    transform: translateY(-5px);
}

.skill-item img {
    width: 60px;
    height: 60px;
    margin-bottom: 10px;
}

/* Projects section styles */
.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
    margin-top: 40px;
}

.project-item {
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 10px;
    overflow: hidden;
    transition: transform 0.3s ease;
}

.project-item:hover {
    transform: translateY(-5px);
}

.project-item img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.project-item h3, .project-item p {
    padding: 20px;
}

/* Contact section styles */
#contact-form {
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 10px;
    padding: 30px;
    max-width: 500px;
    margin: 0 auto;
}

.form-group {
    margin-bottom: 20px;
}

label {
    display: block;
    margin-bottom: 5px;
}

input, textarea {
    width: 100%;
    padding: 10px;
    border: none;
    border-radius: 5px;
    background-color: rgba(255, 255, 255, 0.2);
    color: #ffffff;
}

textarea {
    height: 150px;
    resize: vertical;
}

/* Footer styles */
footer {
    background-color: rgba(0, 0, 0, 0.7);
    backdrop-filter: blur(5px);
    padding: 20px 0;
    text-align: center;
}

.social-links {
    margin-top: 10px;
}

.social-links a {
    color: #ffffff;
    font-size: 24px;
    margin: 0 10px;
    transition: color 0.3s ease;
}

.social-links a:hover {
    color: #3498db;
}

/* Animations */
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes slideUp {
    from { transform: translateY(50px); opacity: 0; }
    to { transform: translateY(0); opacity: 1; }
}

section {
    animation: fadeIn 1s ease-out;
}

.skill-item, .project-item {
    animation: slideUp 0.5s ease-out;
}
    </style>
</head>
<body background="OIP (4).jpg">
    <div class="background-container">
        <img src="OIP (4).jpg" alt="Background GIF">  
    </div>

    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <div class="container">
                <img src="WhatsApp Image 2025-01-29 at 20.59.47_bf5ca714.jpg" alt="PRANEETH SKANDHAN S" class="profile-image">
                <h1>PRANEETH SKANDHAN S</h1>
                <p>Full Stack Developer | UI/UX Enthusiast</p>
                <a href="#contact" class="cta-button">Get In Touch</a>
            </div>
        </section>

        <section id="about">
            <div class="container">
                <h2>About Me</h2>
                <p>Hello! I'm PRANEETH SKANDHAN S, a passionate Full Stack Developer with a keen eye for UI/UX design. I love creating beautiful, functional, and user-friendly web applications that solve real-world problems.</p>
                <p>With expertise in modern web technologies and a strong foundation in computer science, I strive to write clean, efficient, and maintainable code. I'm always eager to learn new technologies and stay up-to-date with the latest industry trends.</p>
                <p>When I'm not coding, you can find me exploring new design trends, contributing to open-source projects, or enjoying a good book on technology and innovation.</p>
            </div>
        </section>

        <section id="skills">
            <div class="container">
                <h2>Skills</h2>
                <div class="skills-grid">
                    <div class="skill-item">
                        <img src="download.jpg" alt="React">
                        <p>React</p>
                    </div>
                    <div class="skill-item">
                        <img src="download (1).jpg" alt="Node.js">
                        <p>Node.js</p>
                    </div>
                    <div class="skill-item">
                        <img src="download (2).jpg" alt="TypeScript">
                        <p>TypeScript</p>
                    </div>
                    <div class="skill-item">
                        <img src="download (3).jpg" alt="Python">
                        <p>Python</p>
                    </div>
                    <div class="skill-item">
                        <img src="download (4).jpg" alt="MongoDB">
                        <p>MongoDB</p>
                    </div>
                    <div class="skill-item">
                        <img src="download (5).jpg" alt="Docker">
                        <p>Docker</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="projects">
            <div class="container">
                <h2>Projects</h2>
                <div class="projects-grid">
                    <div class="project-item">
                        <img src="download (6).jpg" alt="E-commerce Platform">
                        <h3>E-commerce Platform</h3>
                        <p>A full-stack e-commerce solution with React, Node.js, and MongoDB.</p>
                    </div>
                    <div class="project-item">
                        <img src="download (7).jpg" alt="Task Management App">
                        <h3>Task Management App</h3>
                        <p>A responsive task management application built with React and Firebase.</p>
                    </div>
                    <div class="project-item">
                        <img src="download (8).jpg" alt="Weather Forecast Dashboard">
                        <h3>Weather Forecast Dashboard</h3>
                        <p>An interactive weather dashboard using React and OpenWeatherMap API.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <div class="container">
                <h2>Get In Touch</h2>
                <form id="contact-form">
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" required></textarea>
                    </div>
                    <button type="submit" class="cta-button">Send Message</button>
                </form>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2023 PRANEETH SKANDHAN S . All rights reserved.</p>
            <div class="social-links">
                <a href="#" target="_blank"><i class="fab fa-github"></i></a>
                <a href="#" target="_blank"><i class="fab fa-linkedin"></i></a>
                <a href="#" target="_blank"><i class="fab fa-twitter"></i></a>
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
