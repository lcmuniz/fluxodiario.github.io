---
layout: default
title: Início
---

{%- assign posts = site.posts | slice: 0, 5 -%}

{%- for post in posts -%}

  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p><small>{{ post.date | date: "%d %b %Y" }}</small></p>

    {{ post.content }}

    <hr/>

  </article>
{%- endfor -%}

<p style="margin-top:1.5rem;">
  <a href="{{ '/blog/' | relative_url }}">Veja todos os posts →</a>
</p>
