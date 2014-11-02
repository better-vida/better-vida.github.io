---
layout: home
permalink: /
image:
  feature: wood-texture-1600x800.jpg
image:
  folder: 20141025
tags: [wdnica, webdesgin, desarrollo web, pagina web, diseno web, marketing, emarketing, vida, negocios, life, business, tecnologia, technology, html5, lifenbiz, life-and-business, vida-y-negocios]
author: admin
---

<div class="bullets">
	{% for post in site.categories.latest %}
	<div class="bullet three-col-bullet">
		<div class="bullet-icon">
			<a href="{{ site.url }}{{ post.url }}"><img src="{{ site.url }}/images/{{ post.image.teaser }}" alt=""></a>
		</div><!-- /.bullet-icon -->
		<div class="bullet-content">
			<h2><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h2>
			<p>{{ post.excerpt | remove: '<p>' | remove: '</p>'}}</p>
		</div><!-- /.bullet-content -->
	</div><!-- /.bullet -->
	{% endfor %}
</div><!-- /.bullets -->