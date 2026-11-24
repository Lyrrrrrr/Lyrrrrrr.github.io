---
layout: research-home
title: Home
permalink: /
portrait: # Set to the path of an uploaded portrait.
redirect_from:
  - /about/
  - /about.html
---

<section class="hero" aria-labelledby="intro-heading">
  <aside class="profile" aria-label="Academic profile">
    <figure class="portrait"{% unless page.portrait %} aria-hidden="true"{% endunless %}>
      {% if page.portrait %}
        <img src="{{ page.portrait | relative_url }}" alt="Portrait of {{ site.name | escape }}" width="640" height="800" decoding="async">
      {% else %}
        <span class="label">Portrait</span>
      {% endif %}
    </figure>
    <nav class="profile-links" aria-label="Profile links">
      <a href="{{ '/cv/' | relative_url }}">CV</a>
      {% if site.author.github %}<a href="https://github.com/{{ site.author.github | url_encode }}">GitHub</a>{% endif %}
    </nav>
  </aside>
  <div>
    <p class="label">Experimental condensed matter physics</p>
    <h1 id="intro-heading">Superconductivity<br>and magnetism</h1>
    <p class="intro">I am {{ site.name | escape }}, a research assistant at the Tsung-Dao Lee Institute. I study superconductivity and magnetism in quantum materials using muon spectroscopy and computational modelling.</p>
    <div class="actions">
      <a class="button" href="#research">View research</a>
    </div>
    <div class="affiliations">
      <div>
        <p class="label">Current position</p>
        <p><strong>Research Assistant</strong><br>Tsung-Dao Lee Institute<br>Shanghai Jiao Tong University</p>
      </div>
      <div>
        <p class="label">Education</p>
        <p><strong>MPhys (Hons) Physics</strong><br>The University of Manchester</p>
      </div>
    </div>
  </div>
</section>

<section class="research" id="research" aria-labelledby="research-heading">
  <h2 id="research-heading">Research</h2>
  <article class="current-project">
    <div class="current-project-title">
      <p class="label">Current research at TDLI</p>
      <h3>Muon spectroscopy and local magnetism</h3>
    </div>
    <p>I analyse muon spin rotation and relaxation (&mu;SR) data to probe local magnetism in superconducting materials. I fit muon relaxation signals and compare their temperature and field dependence.</p>
  </article>
</section>

<section class="projects" aria-labelledby="projects-heading">
  <h2 id="projects-heading">MPhys projects</h2>
  <div class="project-grid">
    <article class="project">
      <h3>Ising superconductivity in monolayer MoS<sub>2</sub></h3>
      <p>I built a tight-binding model with spin-orbit coupling and a Zeeman term, then solved the linearised gap equation to calculate how the in-plane upper critical field varies with temperature.</p>
    </article>
    <article class="project">
      <h3>Upper critical fields in As<sub>x</sub>P<sub>1&minus;x</sub> thin layers</h3>
      <p>I used a multiband slab model and a finite-thickness Ginzburg-Landau description to study how temperature, field angle and layer thickness affect the upper critical field.</p>
    </article>
  </div>
</section>
