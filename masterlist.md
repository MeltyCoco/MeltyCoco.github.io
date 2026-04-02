---
layout: default
title: Master List
permalink: /masterlist/
---

_**NONE OF THESE TRINKETS ARE CREATED WITH AI**_  
_**EACH TRINKETS SHOW THE ORIGINS OF THE MODEL, THIS INCLUDE 3D MODELER, ARTIST, AND SERIES**_  
_**SUPPORT THE ARTISTS**_  

  

**I'm still in the process of recording all of my trinkets and designing the page by hand ;-;**

<link rel="stylesheet" href="{{ '/assets/css/grid.css' | relative_url }}">

<section class="collection-grid-page">
  <h1>Trinkets!</h1>

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