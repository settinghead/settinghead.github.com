---
layout: page
title: Xiyang Chen's Dev Blog
tagline: ...until I make a better blogging engine for myself.
---
{% include JB/setup %}

## What's in here?

Tech articles.

## Blog
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
