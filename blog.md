---
layout: default
title: Blog
---

# Blog

{% for post in site.posts %}
  ## [{{ post.title }}]({{ post.url }})
  
  {{ post.excerpt }}
  
  Published on {{ post.date | date: "%d %B %Y" }}
  
{% endfor %}
