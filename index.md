---
layout: page
title: settinghead's blog
tagline: Rails, Java, Big Data & shit that matters
---
{% include JB/setup %}

## What's in here?

Mainly tech articles. I share stuff that I think will be beneficial to others.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## Who are you?

Developer, with a streak of a caveman.