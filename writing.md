---
layout: default
title: Writing
permalink: /writing/
---
<div class="writing-header">
  <h1>Writing</h1>
</div>

{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts %}
  <li class="post-list-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="post-list-date">{{ post.date | date: "%b %-d, %Y" }}</span>
  </li>
  {% endfor %}
</ul>
{% else %}
<p>Nothing here yet. Check back soon.</p>
{% endif %}
