---
layout: categorycontents
title: ex423
categories: ['ex423']
showinnav: true
---

<div id="home">
  <ul class="posts">
    {% for post in site.ex423.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>

{% assign selectedcategory = site.categories.ex423 %}
{% include categorycontents %}
