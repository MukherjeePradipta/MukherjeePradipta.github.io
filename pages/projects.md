---
layout: page
title: Projects
permalink: /projects/
---
{% for file in site.static_files %}
  {% if file.path contains '/assets/img/gallery_home/' and (file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.png' or file.extname == '.gif') %}
  
    <img src="{{ file.path }}" alt="Gallery Image">
  {% endif %}
    {% endfor %}


