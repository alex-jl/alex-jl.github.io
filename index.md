---
layout: default
---

<h1>Pages</h1>
<ul>
    <li><a href="ranks">Ranks</a></li>
</ul>

<h1>Blog Posts</h1>
<ul>
  {% for post in site.posts %}
    <li>
        <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> - <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

