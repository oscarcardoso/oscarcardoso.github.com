---
layout: page
title: Code Notes!
tagline: A blog about code notes by Oscar Cardoso
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
	<article>
		<h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
		<h3><span>{{ post.date | date_to_string }}</span></h3>
		{{ post.content }}
		<p><a href="{{ BASE_PATH }}{{ post.url }}">Comments</a></p>
	</article>
  {% endfor %}
</ul>
