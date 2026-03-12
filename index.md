---
layout: default
title: "why not ben"
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <article>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h1>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h1>
        {{ post.content }}
      </article>
    </li>
  {% endfor %}
</ul>
