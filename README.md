<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>About Me</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet"/>
  <style>
    /* Reset and base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Roboto', sans-serif;
      line-height: 1.6;
      background-color: #f0f2f5;
      color: #333;
      transition: background-color 0.3s, color 0.3s;
    }

    /* Dark mode styles */
    body.dark-mode {
      background-color: #121212;
      color: #eee;
    }

    header {
      position: sticky;
      top: 0;
      background-color: #fff;
      padding: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: background-color 0.3s;
    }

    body.dark-mode header {
      background-color: #1e1e1e;
    }

    h1 {
      font-size: 1.8em;
      font-weight: 700;
    }

    /* Toggle button styles */
    .mode-toggle {
      background: none;
      border: 2px solid #333;
      border-radius: 20px;
      padding: 8px 16px;
      cursor: pointer;
      font-size: 0.9em;
      transition: border-color 0.3s, background-color 0.3s;
    }

    body.dark-mode .mode-toggle {
      border-color: #eee;
      color: #eee;
    }

    /* Main container */
    .container {
      max-width: 1200px;
      margin: 30px auto;
      padding: 0 20px;
    }

    /* About Section */
    #about {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 40px;
    }

    .profile-img {
      flex: 1 1 250px;
      max-width: 300px;
      overflow: hidden;
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .profile-img img {
      width: 100%;
      height: auto;
      display: block;
      border-radius: 15px;
    }

    .about-text {
      flex: 2 1 400px;
    }

    .about-text h2 {
      font-size: 2em;
      margin-bottom: 20px;
    }

    .about-text p {
      font-size: 1.1em;
      margin-bottom: 15px;
    }

    /* Skills section */
    #skills {
      margin-top: 50px;
    }

    #skills h3 {
      font-size: 1.8em;
      margin-bottom: 20px;
    }

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 20px;
    }

    .skill {
      background-color: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    body.dark-mode .skill {
      background-color: #2c2c2c;
    }

    .skill:hover {
      transform: translateY(-5px);
      box-shadow: 0 4px 16px rgba(0,0,0,0.2);
    }

    /* Projects section */
    #projects {
      margin-top: 50px;
    }

    #projects h3 {
      font-size: 1.8em;
      margin-bottom: 20px;
    }

    .projects-list {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

    .project {
      background-color: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
    }

    body.dark-mode .project {
      background-color: #2c2c2c;
    }

    .project h4 {
      margin-bottom: 10px;
    }

    .project p {
      font-size: 1em;
    }

    /* Contact section */
    #contact {
      margin-top: 50px;
    }

    #contact h3 {
      font-size: 1.8em;
      margin-bottom: 20px;
    }

    .contact-info {
      display: flex;
      flex-direction: column;
      gap: 15px;
      font-size: 1.1em;
    }

    /* Footer */
    footer {
      margin-top: 60px;
      padding: 20px;
      text-align: center;
      background-color: #fff;
      transition: background-color 0.3s;
    }

    body.dark-mode footer {
      background-color: #1e1e1e;
      color: #eee;
    }

    /* Smooth scroll behavior */
    html {
      scroll-behavior: smooth;
    }

    /* Responsive adjustments */
    @media(max-width: 768px){
      #about {
        flex-direction: column;
      }
      .profile-img {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>About Me</h1>
  <button class="mode-toggle" id="modeToggle">Dark Mode</button>
</header>

<div class="container">

  <!-- About Me Section -->
  <section id="about">
    <div class="profile-img">
      <img src="https://via.placeholder.com/300x300.png?text=My+Photo" alt="My Photo" />
    </div>
    <div class="about-text">
      <h2>Hello! I'm [Your Name]</h2>
      <p>
        Passionate developer with expertise in web development, UI/UX design, and creating interactive experiences. I love turning ideas into reality with code.
      </p>
      <p>
        When I'm not coding, I enjoy exploring new technologies, reading, and traveling to gain inspiration.
      </p>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills">
    <h3>Skills & Technologies</h3>
    <div class="skills-grid">
      <div class="skill">JavaScript</div>
      <div class="skill">HTML5 & CSS3</div>
      <div class="skill">React.js</div>
      <div class="skill">Node.js</div>
      <div class="skill">Python</div>
      <div class="skill">UI/UX Design</div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects">
    <h3>Projects</h3>
    <div class="projects-list">
      <div class="project">
        <h4>Project One</h4>
        <p>A web app that helps users organize their tasks efficiently with real-time collaboration.</p>
      </div>
      <div class="project">
        <h4>Project Two</h4>
        <p>An interactive portfolio website showcasing my work and skills with animations and smooth transitions.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h3>Contact Me</h3>
    <div class="contact-info">
      <div>Email: your.email@example.com</div>
      <div>Phone: +123 456 7890</div>
      <div>Location: Your City, Your Country</div>
    </div>
  </section>

</div>

<!-- Footer -->
<footer>
  &copy; 2024 [Your Name]. All rights reserved.
</footer>

<script>
  // Dark mode toggle
  const toggleButton = document.getElementById('modeToggle');
  toggleButton.addEventListener('click', () => {
    document.body.classList.toggle('dark-mode');
    if(document.body.classList.contains('dark-mode')){
      toggleButton.textContent = 'Light Mode';
    } else {
      toggleButton.textContent = 'Dark Mode';
    }
  });

  // Optional: Animate sections on scroll (using IntersectionObserver)
  const sections = document.querySelectorAll('section');
  const options = {
    threshold: 0.1,
  };

  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if(entry.isIntersecting){
        entry.target.classList.add('visible');
        entry.target.style.opacity = 1;
        entry.target.style.transform = 'translateY(0)';
      } else {
        entry.target.style.opacity = 0;
        entry.target.style.transform = 'translateY(20px)';
      }
    });
  }, options);

  sections.forEach(section => {
    section.style.opacity = 0;
    section.style.transform = 'translateY(20px)';
    section.style.transition = 'all 0.6s ease-out';
    observer.observe(section);
  });
</script>
</body>
</html>
