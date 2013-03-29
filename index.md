---
layout: page
title: Hello World!
tagline: A blog about code notes by Oscar Cardoso
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
	<article>
		<h2>{{ post.title }}</h2>
		<p>{{ post.content }}</p>
		<p><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">Comments</a></p>
	</article>
  {% endfor %}
</ul>
