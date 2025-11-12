---
layout: page
title: Talks
permalink: /talks/
description: #
nav: true
nav_order: 3
display_categories: [research, study groups, outreach]
horizontal: false
---

<!--
These are my upcoming talks:
-->

These are my upcoming talks:

<ul>
<li> <a style= "font-style:italic;">Generalised Kummer surfaces in positive characteristic</a>, <a href="https://www.exeter.ac.uk/events/details/index.php?event=15273">Number Theory, Algebra and Geometry seminar of the University of Exeter</a>.  12th of November, 2025.
</li>
<li> <a style= "font-style:italic;">Pattern detectives: Uncovering the symmetries of designs</a>, <a href="https://warwick.ac.uk/fac/sci/maths/general/outreach/masterclasses/year-12/">Year 12 Masterclass</a>.  28th of February, 2026.</li>
</ul>

These are some of my past talks. And <a href="https://alvarogohe.github.io/blog/2024/pictures_talks/">here</a> are some pictures that my friends took of me while I was giving these talks.

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
