---
layout: about
title: Articles
permalink: /articles/
---

  <ul class="post-list">
  {% for post in site.categories.articles %}
      <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
      <p class="excerpt">{{ post.excerpt }}</p>
      </li>
  {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
