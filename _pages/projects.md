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

These are my upcoming talks:

<ul>
<li><a style="font-weight:bold" href="https://y-rant.github.io/">Crazy for three: Quotients of abelian surfaces by a group of order 3 in characteristic 3</a>, Young Researchers in Algebraic Number Theory, University of Nottingham, 4th September.</li>
<li><a style="font-weight:bold" href="https://math.univ-lille.fr/detail-event/alvaro-gonzalez-hernandez-university-of-warwick-generalised-kummer-surfaces-in-positive-characteristic">Generalised Kummer surfaces in positive characteristic</a>, Université de Lille, 11th September.</li>
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
