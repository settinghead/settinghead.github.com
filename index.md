---
layout: page
title: Xiyang Chen's Dev Blog
tagline: ...until I make a better blogging engine.
---
{% include JB/setup %}

## What's in here?

Tech articles.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## Who are you?

Developer, with a streak of a caveman.
