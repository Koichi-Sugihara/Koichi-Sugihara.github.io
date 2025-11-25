
---
layout: page
title: サイトマップ
permalink: /sitemap/
---
# サイトマップ

## 固定ページ
<ul>
  {% assign pages_sorted = site.pages | sort: "url" %}
  {% for page in pages_sorted %}
    {% if page.sitemap != false and page.url != '/404.html' and page.url != '/' %}
      <li><a href="{{ page.url | relative_url }}">{{ page.title | default: page.url }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

## ブログ記事
<ul>
  {% for post in site.posts %}
    {% if post.sitemap != false %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}（{{ post.date | date: "%Y-%m-%d" }}）</a></li>
    {% endif %}
  {% endfor %}
</ul>
