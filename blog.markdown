---
layout: default
title: Todos os Posts
permalink: /blog/
---

## Todos os posts

<ul>
  {%- for post in site.posts -%}
    <li>
      <span>{{ post.date | date: "%d %b %Y" }}</span>
      — <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {%- endfor -%}
</ul>
