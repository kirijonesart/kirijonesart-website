---
layout: page
title: Gallery
permalink: /gallery/
---

<div class="gallery-grid">
  {% for image in site.data.gallery %}
    <figure class="gallery-item" data-index="{{ forloop.index0 }}">
      <img
        src="{{ '/assets/images/gallery/' | append: image.thumb | relative_url }}"
        data-full="{{ '/assets/images/gallery/' | append: image.file | relative_url }}"
        alt="{{ image.alt | default: 'Artwork' }}"
        loading="lazy"
      />
      {% if image.caption %}<figcaption>{{ image.caption }}</figcaption>{% endif %}
    </figure>
  {% endfor %}
</div>

{% include lightbox.html autoopen=true %}

{% include lightbox.html %}