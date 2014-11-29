---
layout: page
title: Archive
---

## Blog Posts


<ul>
{% for post in site.posts %}
  <li><p>{{ post.date | date_to_string }} &raquo; <a href="{{ post.url }}" target="_self">{{ post.title }}</a></p></li>
{% endfor %}
<ul>
