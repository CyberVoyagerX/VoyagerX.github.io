---
layout: home
title: 欢迎
---

# 欢迎来到我的主页！

这里是我的个人空间，分享技术文章、项目经验和生活点滴。

## 最新文章
{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}

[查看全部文章](/blog) | [关于我](/about)