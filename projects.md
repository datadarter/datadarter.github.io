---
layout: default
title: Selected Blog Posts
---

<div class="row">
  <div class="column">
    {% for post in site.posts %}
      {% if post.selected %}
        <h2>{{ post.title }}</h2>
        <img src="{{ post.image }}" alt="{{ post.title }}" style="width:100%">
        <p>{{ post.excerpt }}</p>
        <p><a href="{{ post.url }}">Read more</a></p>
      {% endif %}
    {% endfor %}
  </div>
  <div class="column">
    {% for post in site.posts %}
      {% if post.selected %}
        <h2>{{ post.title }}</h2>
        <img src="{{ post.image }}" alt="{{ post.title }}" style="width:100%">
        <p>{{ post.excerpt }}</p>
        <p><a href="{{ post.url }}">Read more</a></p>
      {% endif %}
    {% endfor %}
  </div>
</div>
