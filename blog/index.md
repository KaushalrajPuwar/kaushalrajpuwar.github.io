---
layout: default
title: "Blog"
permalink: /blog/
---

# 📝 Blog

Here’s where I document my journey, experiments, and projects.

## Latest Posts

{% assign posts = site.blog | sort: 'date' | reverse | limit: 5 %}
{% for post in posts %}
  <article>
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncate: 150 }}...</p>
    <a href="{{ post.url }}">Read more</a>
  </article>
{% endfor %}
