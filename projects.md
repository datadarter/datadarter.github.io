---
layout: default
title: Selected Blog Posts
---
# Projects


<div class="row">
  <div class="column">
    {% for post in site.posts limit:3 %}
      <h2>{{ post.title }}</h2>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}">Read more</a>
    {% endfor %}
  </div>
  
  <div class="column">
    {% for post in site.posts limit:3 offset:3 %}
      <h2>{{ post.title }}</h2>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}">Read more</a>
    {% endfor %}
  </div>
</div>
