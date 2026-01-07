---
layout: masterlist
title: Master List
permalink: /masterlist/
---
<div class="collection-grid">
  {% for item in site.cosplay_trinkets %}
    <div class="collection-item">
      <a href="{{ item.url | relative_url }}">
        <img src="{{ item.image | relative_url }}" alt="{{ item.title }}">
        <div class="overlay">{{ item.title }}</div>
      </a>
    </div>
  {% endfor %}
</div>