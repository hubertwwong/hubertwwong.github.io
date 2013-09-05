---
title: main page
layout: blog_lists
---
{% for post in site.posts %}
<h2>
	<a href="{{ post.url }}">{{ post.title }}</a>
</h2>
<p class="text-right text-primary">
	{{ post.date | date: "%b %d, %Y" }}
</p>
<p>
	{{ post.excerpt }}
</p>
{% endfor %}