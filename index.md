---
layout: home
permalink: /
image:
  feature: wood-texture-1600x800.jpg
tags: [famila, hijos, padres, ninos, niños, ninas, niñas, adolecentes, infantil, cuidado, educación, educacion, salud, cuidado infantil, aprendizaje, cuidado materno, matenidad, escuela, tareas, dinero, finanzas, hogar, administrar, casa, bebe, bebé, vida, cuidado del hogar, aprendizaje, moda, cuidado personal, ejercicio, tareas, escolar, enfermedad, enfermedades]
author: admin
---
<!-- {% assign category_name = "life" %}
  {% include latest-posts-list-by-category.html %}

{% assign category_name = "business" %}
  {% include latest-posts-list-by-category.html %}
{% include latest-posts-list.html %}
 -->

 <style>
.supcategory {
font-size: 70%;
position: relative;
bottom: 0.3em;
}
</style>
 <h3>Latest</h3>
<ul>
{% for post in site.posts limit:20 %}
<li>
{% if post.date %}
<span>{{ post.date | date: "%B %d, %Y" }}</span> &raquo;
{% endif %}
<a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
<span class="supcategory">{{ post.categories | first }}</span>
</li>
{% endfor %}
</ul>
