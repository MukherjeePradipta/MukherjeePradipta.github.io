---
layout: page
title: Projects
permalink: /projects/
---
{% for image in site.static_files %}
  {% if image.path contains 'assets/img/gallery_all/' %}
    <img src="{{ image.path | relative_url }}" alt="{{ image.name }}">
  {% endif %}
{% endfor %}

