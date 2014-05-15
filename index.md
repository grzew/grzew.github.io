---
layout: default
title: Grzegorz Wieczorek
---

<div id="home">
  <h1>Categories</h1>
      {% for page in site.html_pages %}
        {% if page.title %}
          {% if page.showinnav == true %}
            <a href="{{ page.url | remove:'index.html' }}">{{ page.title }}</a>
          {% endif %}
        {% endif %}
      {% endfor %}
  <br />
  <h1>Last posts</h1>
  <ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>
