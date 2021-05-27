---
layout: default
---

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

[关于](./pages/about.html).

<!--
1，图片 历年变化
2，视频
3，新闻
-->
