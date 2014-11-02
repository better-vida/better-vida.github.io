---
layout: archive
title: "About technologies and how to master it."
date: 2014-05-30T11:40:45-04:00
modified:
excerpt: "Use the technology, don't let technology use you."
tags: []
image:
  feature:
  teaser:
---

<div class="tiles">
{% for post in site.categories.technology %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->