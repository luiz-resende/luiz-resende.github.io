---
layout: page
permalink: /repositories/
title: repositories
description: My GitHub profile and repositories. # Edit in `_data/repositories.yml`
nav: true # Whether (`true`) or not (`false`) to show this section
nav_order: 5 # The order in the navegation bar ("about" is assumed as 0)
---

## GitHub user

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>
{% endif %}

---

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
