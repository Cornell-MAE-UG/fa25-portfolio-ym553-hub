---
layout: default
title: Projects
permalink: /projects/

<h1>Projects</h1>
<ul>
  {% for project in site.projects %}
    <li><a href="{{ project.url | relative_url }}">{{ project.title }}</a></li>
  {% endfor %}
</ul>
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title}}</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>