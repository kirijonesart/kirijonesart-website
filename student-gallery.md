---
layout: page
title: Student Gallery
permalink: /student-gallery/
---

A rotating selection of student and instructor artworks.

<div class="gallery-grid">
  {% for image in site.data.student-gallery %}
    <figure>
      <img src="{{ '/assets/images/student-gallery/' | append: image.file | relative_url }}" alt="{{ image.alt }}" loading="lazy" />
      {% if image.caption %}<figcaption>{{ image.caption }}</figcaption>{% endif %}
    </figure>
  {% endfor %}
</div>
