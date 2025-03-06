---
layout: home
title: 博客
permalink: /blog
---

# 所有文章

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}