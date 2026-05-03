---
layout: default
title: Recipes
---

# 🍽 Recipes

<p class="intro">
Browse simple, practical recipes.
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