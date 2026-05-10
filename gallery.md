---
layout: page
title: Gallery
permalink: /gallery/
---

A rotating selection of student and instructor artworks.

<div class="gallery-grid">
  {% for image in site.data.gallery %}
    <figure>
      <img src="{{ '/assets/images/' | append: image.file | relative_url }}" alt="{{ image.alt }}" loading="lazy" />
      {% if image.caption %}<figcaption>{{ image.caption }}</figcaption>{% endif %}
    </figure>
  {% endfor %}
</div>
