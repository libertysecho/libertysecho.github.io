---
layout: page
title: Articles
permalink: /articles/
---

{% for page in site.pages %}
  {% if page.url contains '/articles/' and page.title and page.url != '/articles/' %}
  - [{{ page.title }}]({{ page.url | relative_url }})
  {% endif %}
{% endfor %}