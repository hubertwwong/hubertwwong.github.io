---
title: Hello World!!!!
layout: blog
---
<ul>
  {% for post in site.posts %}
    <h6>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h6>
    <p>{{ post.excerpt }}</p>
  {% endfor %}
</ul>