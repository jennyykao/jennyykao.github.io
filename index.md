---
layout: default
---

<header class="site-header">
  <nav class="nav">
    <ul>
      <li><a href="/">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<section class="hero">
  <h1>Your Name</h1>
  <p>Your tagline or short description</p>
</section>

<section id="about" class="about">
  <h2>About Me</h2>
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
