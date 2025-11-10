---
layout: default
title: ホーム
---

# 河野 健

修士1年
このサイトでは、簡単な自己紹介と、日々の学びやアウトプットをまとめるテックブログを掲載します。

## 自己紹介
- 専門: Web/クラウド/アプリケーション開発
- 関心: アーキテクチャ設計、パフォーマンス最適化、開発体験改善
- 拠点: 日本（JST）

## 技術スタック
- 言語: TypeScript / JavaScript / Python / Go など
- フレームワーク: React / Next.js / Node.js / FastAPI など
- インフラ: AWS / GCP / Docker / Kubernetes（必要に応じて）

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


