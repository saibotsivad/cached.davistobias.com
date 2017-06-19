---
layout: index
isroot: true
---


<header class="index">
	<h1>{{ site.name }}</h1>
	<p>{{ site.description }}</p>
	<hr>
</header>

<ul>
{% for post in site.pages %}{% if post.published == true %}
	<li>
		<a href="{{ post.url | replace:'.html','' }}">{{ post.title | xml_escape }}</a>
	</li>
{% endif %}{% endfor %}
</ul>
