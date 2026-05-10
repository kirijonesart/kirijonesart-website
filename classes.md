---
layout: page
title: What I Offer
permalink: /classes/
---

I offer a range of art experiences designed to suit different ages, abilities, and occasions. Whether you’re looking to learn, celebrate, or commission something unique, there’s something here for you.

## Art Classes

Regular art classes provide a calm and supportive space to explore drawing and painting. These sessions are suitable for beginners as well as those with more experience. You’ll be guided at your own pace, with a focus on building confidence, developing skills, and enjoying the creative process.

Browse our current and upcoming classes. Click a class to learn more.

<ul class="class-list">
  {%- assign classes = site.classes | sort: 'title' -%}
  {%- for c in classes -%}
    <li>
      <a href="{{ c.url | relative_url }}">{{ c.title }}</a>
      {%- if c.level %} <span class="badge level">{{ c.level }}</span>{% endif %}
      {%- if c.schedule %} <span class="schedule">{{ c.schedule }}</span>{% endif %}
    </li>
  {%- endfor -%}
</ul>

## 1:1 Tuition

One-to-one sessions offer a more personalised approach, tailored entirely to you. Whether you’d like to focus on specific techniques, build a scholarship portfolio, or simply gain confidence, these sessions are designed around your individual goals and interests.

## Art Parties

Art parties are a relaxed and creative way to celebrate a special occasion. Suitable for both children and adults, these sessions are fun, informal, and designed so everyone can enjoy making something to take home—no experience needed.
