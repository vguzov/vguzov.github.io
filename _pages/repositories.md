---
layout: page
permalink: /repositories/
title: repositories
description: 
nav: true
nav_order: 4
header_title: Selected GitHub Repositories
---

[//]: # (## Selected GitHub Repositories)

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
