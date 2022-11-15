---
layout: default
---
<section class="hero">
  <div class="hero-inside">
    <div class="hero-text">
      <h2>We build websites.</h2>
      <p>We specialize in branding, website design, WordPress development, and technology integration for small businesses and nonprofits.</p>
      <p><a href="mailto:ryan@fourteensquare.com">Get in touch.</a></p>
    </div>
    <div class="hero-illustration">
      {% include hero-illustration.html %}
    </div>
  </div>
</section>

<section class="projects">
  <ul class="project-list">
  {% for project in site.data.projects %}
    <li class="project-item">
      <a href="{{ project.url }}">
        <img class="project-screenshot" src="/assets/img/{{ project.screenshot }}" alt="Screenshot of {{ project.name }} website" />
      </a>
      <h2 class="project-name">
        <a href="{{ project.url }}">
          {{ project.name }}
        </a>
      </h2>
      <p class="project-skills">{{ project.skills }}</p>
    </li>
  {% endfor %}
  </ul>
</section>