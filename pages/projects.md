---
layout: page
title: Projects
permalink: /projects/
---
{% for image in site.static_files %}
  {% if image.path contains 'assets/img/' %}
    <img src="{{ site.baseurl }}{{ image.path }}" alt="{{ image.name }}">
  {% endif %}
{% endfor %}
