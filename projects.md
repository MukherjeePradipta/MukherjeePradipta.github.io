---
layout: page
title: Projects
---

<style>
  .image-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 5px;
  }
  .image-grid img {
    max-width: 100%;
    height: auto;
  }
</style>

<div class="image-grid">
  {% for file in site.static_files %}
    {% if file.path contains '/assets/img/gallery_home/' and (file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.png' or file.extname == '.gif') %}
      <img src="{{ file.path }}" alt="Gallery Image">
    {% endif %}
  {% endfor %}
</div>
