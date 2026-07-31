---
layout: page
permalink: /code/
title: Code
nav: false
nav_order: 4
---

I try to keep updated all the coding that I do in my GitHub.

{% if site.data.repositories.github_users %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>
{% endif %}


These are some of my repositories:

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}

<div style="padding-bottom: 100px; padding-top: 100px;">
<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/Website_developer.jpg" title="Me developing a website" class="img-fluid rounded z-depth-1" width="80%" %}
    </div>
</div>
<div class="caption">
    I also made this website (with <a href="https://github.com/alshedivat/al-folio/tree/main">some help</a>)!
</div>
</div>

