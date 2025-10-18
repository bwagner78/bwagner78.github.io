---
layout: default
title: Tags
permalink: /tags/
---

<h1>All Tags</h1>
<ul>
{% for tag in site.tags %}
  <li>
    <a href="{{ '/tag/' | append: tag[0] | slugify | append: '/' | relative_url }}">
      {{ tag[0] }} ({{ tag[1].size }})
    </a>
  </li>
{% endfor %}
</ul>