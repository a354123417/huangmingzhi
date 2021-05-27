---
layout: default
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

[Link to about page](./pages/about.html).

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

# 黄明志

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
