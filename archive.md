---
layout: page
title: Archives
---
<ul>
{% for post in site.posts %}
  <li>
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
  </li>
{% endfor %}
<ul>