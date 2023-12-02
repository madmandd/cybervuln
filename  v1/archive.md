---
title: archive
layout: page
permalink: /archive/
---

{% for post in site.posts %}
{% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
{% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
{% if year != nyear %}
{% if forloop.index0 != 0 %}
</ul>
{% endif %}
<h2>{{ post.date | date: '%Y' }}</h2><ul>
{% endif %}

  <li><a href="{{ post.url }}">{{ post.title }}</a><br><time datetime="{{ post.date | date: "%Y-%m-%d" }}T{{ post.date | date: "%H:%M" }}">{{ post.date | date: "%B %d, %Y" }}</time></li>
{% endfor %}
