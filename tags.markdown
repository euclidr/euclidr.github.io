---
layout: page
title: Tag
permalink: /tag/
---
<ul>
{% for tag in site.tags %}
  <li><a href="{{ site.baseurl }}/tag/{{ tag[0] }}/index.html">{{ tag[0] }}</a></li>
{% endfor %}
</ul>