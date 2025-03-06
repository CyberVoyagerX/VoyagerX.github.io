---
layout: default
{{ site.title }}
---

# 欢迎来到 {{ site.title }}！

这里是文档中心，以下是推荐阅读的内容：

## 快速入门
1. [安装指南]({{ site.baseurl }}/docs/doc1)
2. [使用教程]({{ site.baseurl }}/docs/doc2)

## 所有文档
<ul>
  {% for doc in site.pages %}
    {% if doc.path contains 'docs/' %}
      <li>
        <a href="{{ doc.url | relative_url }}">{{ doc.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>