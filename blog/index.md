---
layout: default
title: Blaaug
curr: blog
---
{% for post in site.posts %}

* ### {{ post.date | date: "%Y %b %d" }}
	<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
	{{ post.content | truncatewords: 40 }}
{% endfor %}