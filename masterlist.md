---
layout: default
title: Portfolio
permalink: /masterlist/
---

<link rel="stylesheet" href="{{ '/assets/css/grid.css' | relative_url }}">

<section class="collection-grid-page">
  <h1>Why tho</h1>

  <div class="grid">
    {% for item in site.cosplay_trinkets %}
      <a class="card" href="{{ item.url }}">
        <div class="card-image">
          {% if item.image %}
            <img src="{{ item.image }}" alt="{{ item.title }}">
          {% else %}
            <div class="card-placeholder">No Image</div>
          {% endif %}
        </div>
        <div class="card-body">
          <h2>{{ item.title }}</h2>
          {% if item.description %}
            <p>{{ item.description }}</p>
          {% endif %}
        </div>
      </a>
    {% endfor %}
  </div>
</section>