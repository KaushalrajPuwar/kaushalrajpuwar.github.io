---
layout: default
title: "Blog"
permalink: /blog/
---

# 📝 Blog

Here’s where I document my journey, experiments, and projects.  

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) – {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
