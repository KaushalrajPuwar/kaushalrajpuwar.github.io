---
layout: default
title: "Blog"
permalink: /blog/
---

# 📝 Blog

Here’s where I document my journey, experiments, and projects.

<ul>
{% for post in site.posts %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> – {{ post.date | date: "%B %d, %Y" }}</li>
{% endfor %}
</ul>
