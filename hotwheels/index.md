---
layout: default
title: Hotwheels
---

# 🍽 HotWheels

<p class="intro">
Looks at cool hot wheels pictures.
</p>

<ul class="recipe-list">
  {% for page in site.pages %}
    {% if page.path contains "recipes/" and page.name != "index.md" %}
      <li>
        <a href="{{ page.url | relative_url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>