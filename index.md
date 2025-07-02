---
layout: default
---

<head>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;700&display=swap" rel="stylesheet">
<style>
  code, pre {
    font-family: 'Fira Code', monospace;
  }
</style>
</head>

<header class="site-header">
  <nav class="nav">
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#portfolio">Projects</a></li>
      <li><a href="/articles.html">Posts</a></li>
      <li><a href="/categories.html">Categories</a></li>
      <li><a href="/tags.html">Tags</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<section class="hero">
  <img src="/assets/images/profile-pic.jpg" alt="Jenny Kao headshot" class="profile-pic">
  <p> hi there, hello <span class="wave">👋</span>&ensp;this is</p>
  <h1>&lt;Jenny&ensp;Kao&gt;</h1>
  <div class="hero-actions">
    <div class="hero-social">
      <a href="https://linkedin.com/in/yourusername" target="_blank"><i class="fab fa-linkedin"></i></a>
      <a href="https://github.com/yourusername" target="_blank"><i class="fab fa-github"></i></a>
    </div>
    <div class="hero-buttons">
      <a href="/assets/resume.pdf" class="button" target="_blank">Resume</a>
      <a href="mailto:youremail@example.com" class="button">Email Me</a>
    </div>
    
  </div>
</section>

<section id="about" class="about">
  <h2>👩🏻‍💻 The Cliff Notes on Me</h2>
  <p>Write a brief introduction about yourself here.</p>
</section>

<section id="portfolio" class="portfolio">
  <h2>📊 Projects</h2>
  <div class="project-grid">
    {% for project in site.data.projects %}
    <div class="project-card">
      <a href="{{ project.url }}" target="_blank">
        <img src="{{ project.image }}" alt="{{ project.title }}">
        <h3>{{ project.title }}</h3>
      </a>
      <p>{{ project.description }}</p>
    </div>
    {% endfor %}
  </div>
</section>

<section id="experience" class="experience">
  <h2>📍I’ve worked in tech companies, startups and non-profit organizations.</h2>
  <div class="experience-grid">
    {% for job in site.data.work %}
    <div class="experience-item">
      <h3>{{ job.title }}</h3>
      <p>{{ job.company }}</p>
    </div>
    {% endfor %}
  </div>
  <div class="resume-button">
    <a href="/assets/resume.pdf" target="_blank" class="button">Resume</a>
  </div>
</section>

<section id="contact" class="contact">
  <div class="contact-container">
    <div class="contact-image">
      <img src="/assets/images/contact.jpg" alt="Contact">
    </div>
    <div class="contact-content">
      <h2>Say hello 🙌 Let's Connect! </h2>
      <p>If you’d like to get in touch, feel free to email me or connect via LinkedIn and GitHub.</p>
      <p>
        <a href="mailto:youremail@example.com" class="button">Email Me</a>
      </p>
    
    </div>
  </div>
  </section>

<footer class="site-footer">
  <p> &copy; 2025 Your Name. All rights reserved.</p>
</footer>
