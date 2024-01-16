---
layout: page
title: Projects
permalink: /projects/
description: A selected collection of my projects.
cover_image: /assets/img/cover.png
nav: true
nav_order: 3
horizontal: false

---

---

<!-- pages/projects.md -->
<div class="projects">
{% if site.projects %}
  <!-- Display all projects without categories -->
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% for project in sorted_projects %}
    {% include project_card.html %}
        <hr style="margin: 20px 0;">

  {% endfor %}
{% endif %}
</div>
