---
layout: page
title: Student Gallery
permalink: /student-gallery/
---

A selection of student artworks.

<div class="gallery-grid">
  {% for image in site.data.student-gallery %}
    <figure class="gallery-item" data-index="{{ forloop.index0 }}">
      <img
        src="{{ '/assets/images/student-gallery/' | append: image.thumb | relative_url }}"
        data-full="{{ '/assets/images/student-gallery/' | append: image.file | relative_url }}"
        alt="{{ image.alt | default: 'Student artwork' }}"
        loading="lazy"
      />
      {% if image.caption %}<figcaption>{{ image.caption }}</figcaption>{% endif %}
    </figure>
  {% endfor %}
</div>

{% include lightbox.html %}
