---
layout: default
title: Blog
---

{% for post in site.posts %}
  <div class="post">
    <h1>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></h1>
    {{ post.content }}
    <small>Written by {{ post.author }}</small>
  </div>
{% endfor %}
