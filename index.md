---
layout: default
title: 黄明志 namewee
---

## MV (横6个)
<ul>
    <li>[黃明志Namewee feat. 王力宏 Leehom Wang【漂向北方 Stranger In The North 】@CROSSOVER ASIA 2017亞洲通車專輯](https://www.youtube.com/watch?v=qIF8xvSA0Gw)</li>
    <li>[黃明志【東京盆踊りTokyo Bon 2020】Ft. 二宮芽生 & Cool Japan TV @亞洲通吃 2018 All Eat Asia](https://www.youtube.com/watch?v=zhGnuWwpNxI)</li>
    <li>[洗腦神曲【好想你】四葉草 @RED People](https://www.youtube.com/watch?v=fdQgPu3iUYk)</li>
    <li>[黃明志 Ft. 鄧紫棋【漂向北方】KTV 包廂版 @2017](https://www.youtube.com/watch?v=YJSpGXxkCqE)</li>
    <li>[黃明志泰國情哥Part 3!【泰國恰恰】Ft. Bie The Ska บี้เดอะสกา @亞洲通吃 2017 All Eat Asia](https://www.youtube.com/watch?v=YaZ5eV9BEX8)</li>
    <li>[黃明志用中文唱泰語【泰國情哥】@亞洲通緝 2013 Asia Most Wanted](https://www.youtube.com/watch?v=SwZMS-ISbH4)</li>
</ul>

<ul class="post-list">
    {% for article in site.articles %}
      <li>

        {% assign date_format = site.cayman-blog.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ article.date | date: date_format }}</span>

        <h2>
          <a class="post-link" href="{{ article.url | absolute_url }}" title="{{ article.title }}">{{ article.title | escape }}</a>
        </h2>

        {{ article.excerpt | markdownify | truncatewords: 30 }}

      </li>
    {% endfor %}
</ul>

## 文章 (左右两列 每列6个)
<ul class="post-list">
    {% for post in site.posts %}
      <li>

        {% assign date_format = site.cayman-blog.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ post.date | date: date_format }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | absolute_url }}" title="{{ post.title }}">{{ post.title | escape }}</a>
        </h2>

        {{ post.excerpt | markdownify | truncatewords: 30 }}

      </li>
    {% endfor %}
</ul>

## 电影 (横3?个)
[黃明志電影 你是豬 (2020) MOVIE Babi]()
[黃明志電影 鬼老大哥大 (2012) MOVIE Hantu Gangster]()
[黃明志電影 辣死你媽 (2011) MOVIE Nasi Lemak 2.0]()

## 图片 ()

[关于](./pages/about.html).

<!--
1，图片 历年变化
2，视频
3，新闻
-->
