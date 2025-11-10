---
layout: default
title: Code de Note
---

こんにちは、東京科学大学修士1年の 河野 健 といいます。専門は画像処理AIです。
このサイトでは、簡単な自己紹介と、日々の学びやアウトプットをまとめるテックブログを掲載します。

## 自己紹介
- 専門: 画像処理、特に物体検出に関する半教師あり学習。楽譜転写AIの開発とかも。
- 関心: AI/機械学習/信号処理/アルゴリズム
- 拠点: 日本（JST）


## ブログ
- 記事一覧は「[ブログ](/blog/)」からご覧ください。

## 最近の投稿
{% assign recent_posts = site.posts | slice: 0, 5 %}
{% if recent_posts.size > 0 %}
<ul>
  {% for post in recent_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small> - {{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
  </ul>
{% else %}
まだ投稿はありません。はじめての投稿をお楽しみに！
{% endif %}


