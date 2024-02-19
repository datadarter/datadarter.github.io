---
layout: default
title: Blog
---

# Blog

{% for post in site.posts %}
  [{{## post.title }}]({{ post.url }})
  <p>{{ post.excerpt }}</p>
  <p>Published on {{ post.date | date: "%d %B %Y" }}</p>
  <hr>
{% endfor %}
