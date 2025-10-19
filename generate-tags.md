---
layout: null
permalink: /generate_tags/
---

{% for tag in site.tags %}
  {% capture tag_name %}{{ tag[0] }}{% endcapture %}
  ---
  layout: tag
  tag: {{ tag_name }}
  permalink: /tags-{{ tag_name | slugify }}/
  ---
{% endfor %}