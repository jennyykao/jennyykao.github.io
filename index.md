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
  <h2>Portfolio</h2>
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

<section id="contact" class="contact">
  <h2>Contact</h2>
  <p>Include your email or links to your profiles.</p>
</section>

<footer class="site-footer">
  <p>&copy; 2025 Your Name. All rights reserved.</p>
  <p>
    <a href="mailto:youremail@example.com">Email</a> |
    <a href="https://www.linkedin.com/in/yourusername" target="_blank">LinkedIn</a> |
    <a href="https://github.com/yourusername" target="_blank">GitHub</a>
  </p>
</footer>
