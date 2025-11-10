---
layout: default
title: ブログ
permalink: /blog/
---

# ブログ

技術系の学びや調査メモ、開発のベストプラクティスなどを投稿します。

{% if site.posts and site.posts != empty %}
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small> - {{ post.date | date: "%Y-%m-%d" }}</small><br/>
      {% if post.excerpt %}
        <span>{{ post.excerpt | strip_html | truncate: 120 }}</span>
      {% endif %}
    </li>
  {% endfor %}
  </ul>
{% else %}
まだ投稿がありません。
{% endif %}


