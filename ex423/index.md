---
layout: categorycontents
title: ex423
categories: ['ex423']
showinnav: true
---

<div id="home">
  <p>
   The Red Hat® Enterprise Directory Services and Authentication Expertise Exam is a performance-based test of the skills covered in Red Hat Enterprise Directory Services and Authentication (RH423). To enroll in this exam, candidates must hold a current Red Hat Certified Engineer (RHCE®) certification.
  </p><p>
   <a href="http://www.redhat.com/training/courses/ex423/examobjective">exam objective</a>
  </p>
  <ul class="posts">
    {% for post in site.ex423.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>
