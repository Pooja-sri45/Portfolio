# Ex01 Portfolio
## Date:13/08/2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Portfolio</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <!-- Header -->
    <header>
        <div class="logo">Poojasri L</div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-text">
            <h1>Hello, I'm <span>POOJASRI</span></h1>
            <p>3rd Year IT Student | Aspiring Full Stack Developer</p>
            <a href="#projects" class="btn">View My Work</a>
        </div>
        <div class="hero-img">
            <img src="sri.jpg" alt="Pooja Profile Picture" />
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <p>
            I am currently pursuing a B.Tech degree in Information Technology at Saveetha Engineering College. 
            I have a strong interest in Data Science and Web Development, and I am eager to apply my theoretical 
            knowledge in practical settings.I am keen on exploring opportunities for skill development and professional
            growth within the technology sector, with a focus on contributing to innovative projects and earning 
            industry-relevant certifications.Passionate about technology, I enjoy learning new tools and frameworks
            to build interactive web applications.
        </p>
    </section>

    <!-- Skills Section -->
    <!-- Skills Section -->
    <section id="skills">
        <h2>Skills</h2>
        <div class="skills-grid">
            <div>Java</div>
            <div>C</div>
            <div>Python</div>
            <div>HTML</div>
            <div>CSS</div>
            <div>JavaScript</div>
            <div>React</div>
            <div>UiPath</div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>Projects</h2>
        <div class="project-list">
            <div class="project-card">
                <h3>Portfolio Website</h3>
                <p>Responsive personal website built with HTML, CSS, and JavaScript.</p>
            </div>
            <div class="project-card">
                <h3>Local Business Website</h3>
                <p>Website for a local business with booking and contact features.</p>
            </div>
            <div class="project-card">
                <h3>Software Company Website</h3>
                <p>Professional company site with modern UI.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:sri249623@gmail.com">sri249623@gmail.com</a></p>
        <p>GitHub: <a href="https://github.com/Pooja-sri45" target="_blank">github.com/Pooja-sri45</a></p>
        <p>LinkedIn: <a href="https://www.linkedin.com/in/poojasri-l-298ab3338/" target="_blank">linkedin.com/in/poojasri-l</a></p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Poojasri | All Rights Reserved</p>
    </footer>
</body>
</html>
```
style.css

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #f4f4f4;
    color: #333;
    line-height: 1.6;
    scroll-behavior: smooth;
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #222222;
    color: #fff;
    padding: 1rem 2rem;
    position: sticky;
    top: 0;
    z-index: 1000;
}

header .logo {
    font-size: 1.5rem;
    font-weight: bold;
}

nav a {
    color: #fff;
    margin-left: 1rem;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    color: #ff00b3;
}

/* Hero Section */
.hero {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    padding: 3rem 2rem;
    background: linear-gradient(to right, #00c3ff, #00e5ff);
    color: #222;
}

.hero-text {
    max-width: 500px;
    margin-right: 2rem;
}

.hero-text h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.hero-text span {
    color: #fff;
}

.btn {
    display: inline-block;
    margin-top: 1rem;
    padding: 0.7rem 1.5rem;
    background: #222;
    color: #fff;
    border-radius: 5px;
    text-decoration: none;
}

.btn:hover {
    background: #444;
}

.hero-img img {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    object-fit: cover;
    box-shadow: 0 2px 8px rgba(0,0,0,0.2);
}

/* Sections */
section {
    padding: 2rem;
    text-align: center;
}

h2 {
    margin-bottom: 1rem;
    color: #222;
}

/* Skills */
.skills-grid {
    
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-top: 1rem;
    justify-content: center;
}

.skills-grid div {
    background: #fff;
    padding: 1rem;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    font-weight: bold;
}

/* Projects */
.project-list {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: center;
}

.project-card {
    background: #fff;
    padding: 1rem;
    width: 300px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.project-card h3 {
    margin-bottom: 0.5rem;
}

/* Footer */
footer {
    background: #222;
    color: #fff;
    text-align: center;
    padding: 1rem;
}

/* Responsive */
@media (max-width: 768px) {
    .hero {
        flex-direction: column;
        text-align: center;
    }
    .hero-text {
        margin-right: 0;
    }
}

```


## OUTPUT
<img width="1919" height="1016" alt="Screenshot 2025-08-11 220343" src="https://github.com/user-attachments/assets/521e8245-9edf-429d-8e9e-9b0ad367c4b3" />
<img width="1919" height="1077" alt="Screenshot 2025-08-11 220356" src="https://github.com/user-attachments/assets/ea404c3c-1c5c-4c25-9c5e-17ada8103dc8" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
