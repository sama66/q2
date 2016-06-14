---
layout: maestros
title: Maestros
permalink: /maestros/
---

   <ul class="maestro-list">
   {% for post in site.categories.maestros %}
       <li><a href="{{ post.url | prepend: site.baseurl }}"><img src="{{ site.baseurl }}/img/small/{{ post.img.small }}"><br/>{{ post.title }}</a></li>
   {% endfor %}
  </ul>
