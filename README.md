# Prabhat.github<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Prabhat Kumar Yadav - Portfolio</title>
  <style>
    /* Reset and base */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.1;
      background: #f9f9f9;
      color: #333;
      scroll-behavior: smooth;
    }
    a {
      color: #0077b6;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }

    /* Container */
    .container {
      max-width: 1000px;
      margin: auto;
      padding: 0 20px;
    }

    /* Header & Nav */
    header {
      background: #023e8a;
      color: #fff;
      padding: 20px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .container-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      font-size: 1.5rem;
      font-weight: 700;
      letter-spacing: 1px;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
    }
    nav ul li {
      font-weight: 600;
    }
    nav ul li a {
      color: #caf0f8;
      font-size: 1rem;
      transition: color 0.3s ease;
    }
    nav ul li a:hover,
    nav ul li a.active {
      color: #90e0ef;
      border-bottom: 2px solid #90e0ef;
      padding-bottom: 2px;
    }

    /* Hamburger menu for mobile */
    .hamburger {
      display: none;
      flex-direction: column;
      cursor: pointer;
      gap: 5px;
    }
    .hamburger div {
      width: 25px;
      height: 3px;
      background: #caf0f8;
      border-radius: 2px;
    }

    /* Sections */
    section {
      padding: 60px 0;
    }
    h1, h2 {
      margin-bottom: 15px;
      color: #023e8a;
    }
    h1 {
      font-size: 2.5rem;
    }
    h2 {
      font-size: 2rem;
      border-bottom: 3px solid #90e0ef;
      display: inline-block;
      padding-bottom: 5px;
      margin-bottom: 30px;
    }
    p {
      font-size: 1.1rem;
      max-width: 700px;
    }

    /* Home Section */
    #home {
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 80vh;
      text-align: center;
      background: linear-gradient(135deg, #90e0ef 0%, #caf0f8 100%);
      color: #03045e;
      padding: 0 20px;
    }
    #home h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }
    #home p {
      font-size: 1.3rem;
      font-weight: 600;
    }

    /* About Section */
    #about p {
      max-width: 700px;
      font-size: 1.15rem;
      line-height: 1.7;
      color: #333;
    }

    /* Skills Section */
    #skills ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      max-width: 700px;
    }
    #skills ul li {
      background: #90e0ef;
      color: #03045e;
      padding: 10px 20px;
      border-radius: 25px;
      font-weight: 600;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      transition: background 0.3s ease;
    }
    #skills ul li:hover {
      background: #0077b6;
      color: #caf0f8;
      cursor: default;
    }

    /* Projects Section */
    #projects .project-list {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      max-width: 700px;
    }
    #projects .project {
      background: #caf0f8;
      border-radius: 10px;
      padding: 20px;
      flex: 1 1 300px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }
    #projects .project:hover {
      transform: translateY(-5px);
    }
    #projects .project h3 {
      margin-bottom: 10px;
      color: #0077b6;
    }
    #projects .project p {
      font-size: 1rem;
      color: #03045e;
    }

    /* Contact Section */
    #contact p {
      font-size: 1.1rem;
      margin-bottom: 10px;
    }
    #contact a {
      display: inline-block;
      margin-right: 15px;
      font-weight: 600;
      color: #0077b6;
      transition: color 0.3s ease;
    }
    #contact a:hover {
      color: #023e8a;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px 0;
      background: #023e8a;
      color: #caf0f8;
      font-size: 0.9rem;
    }

    /* Responsive */
    @media (max-width: 768px) {
      nav ul {
        position: fixed;
        top: 70px;
        right: -100%;
        background: #023e8a;
        height: calc(100% - 70px);
        width: 200px;
        flex-direction: column;
        padding-top: 20px;
        gap: 20px;
        transition: right 0.3s ease;
        z-index: 999;
      }
      nav ul.active {
        right: 0;
      }
      .hamburger {
        display: flex;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="container container-header">
      <div class="logo">Prabhat Kumar Yadav</div>
      <nav>
        <ul id="nav-links">
          <li><a href="#home" class="active">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <div class="hamburger" id="hamburger">
        <div></div>
        <div></div>
        <div></div>
      </div>
    </div>
  </header>

  <main>
    <section id="home">
      <h1>Prabhat Kumar Yadav</h1>
      <p>Aspiring Computer Science Engineer | AIML Enthusiast</p>
    </section>

    <section id="about" class="container">
      <h2>About Me</h2>
      <p>
        I’m Prabhat Kumar Yadav, a passionate learner and aspiring Computer Science Engineer with interest in Artificial Intelligence, Machine Learning, and Web Development. I love coding, solving problems, and turning ideas into reality.
      </p>
    </section>

    <section id="skills" class="container">
      <h2>Skills</h2>
      <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>Python</li>
        <li>C++</li>
        <li>AIML</li>
      </ul>
    </section>

    <section id="projects" class="container">
      <h2>Projects</h2>
      <div class="project-list">
        <div class="project">
          <h3>Portfolio Website</h3>
          <p>A personal portfolio website showcasing my skills and projects.</p>
  
      </div>
    </section>

    <section id="contact" class="container">
      <h2>Contact</h2>
      <p>Email: <a href="mailto:yadavprabhatkumar2007@gma">yadavprabhatkumar2007@gma</a></p>
      <p>
        LinkedIn: 
        <a href="https://www.linkedin.com/in/prabhat-kumar-yadav-836477356?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank" rel="noopener noreferrer">
          prabhat-kumar-yadav
        </a>
      </p>
      <p>GitHub: <a href="#" aria-disabled="true" title="GitHub link not provided">Coming Soon</a></p>
    </section>
  </main>

  <footer>
    &copy; 2024 Prabhat Kumar Yadav. All rights reserved.
  </footer>

  <script>
    // Mobile menu toggle
    const hamburger = document.getElementById('hamburger');
    const navLinks = document.getElementById('nav-links');

    hamburger.addEventListener('click', () => {
      navLinks.classList.toggle('active');
    });

    // Close menu on link click (mobile)
    navLinks.querySelectorAll('a').forEach(link => {
      link.addEventListener('click', () => {
        navLinks.classList.remove('active');
      });
    });

    // Highlight active nav link on scroll
    const sections = document.querySelectorAll('section');
    const navItems = document.querySelectorAll('nav ul li a');

    window.addEventListener('scroll', () => {
      let current = '';
      sections.forEach(section => {
        const sectionTop = section.offsetTop - 80;
        if (pageYOffset >= sectionTop) {
          current = section.getAttribute('id');
        }
      });
      navItems.forEach(a => {
        a.classList.remove('active');
        if (a.getAttribute('href') === '#' + current) {
          a.classList.add('active');
        }
      });
    });
  </script>
</body>
</html>
