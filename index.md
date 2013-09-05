---
title: main page
layout: blog_lists
---
<div class="row">
	{% for post in site.posts %}
	<div class="col-md-12 spacer_bottom">
		<h2>
			<a href="{{ post.url }}">{{ post.title }}</a>
		</h2>
		<p class="text-right text-primary">
			{{ post.date | date: "%b %d, %Y" }}
		</p>
		<p>
			{{ post.excerpt }}
		</p>
		<p class="text-warning">
			tags:
			{{ post.tags }}
		</p>
	</div>
	{% endfor %}
</div>