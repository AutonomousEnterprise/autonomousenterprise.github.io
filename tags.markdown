---
layout: page
title: Tags
permalink: /tags/
---

{% assign tags = site.tags | sort %}

{% for tag in tags %}
### <a id="{{ tag[0] | slugify }}"></a>{{ tag[0] }}

<ul>
  {% for post in tag[1] %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%Y-%m-%d" }})</small>
    </li>
  {% endfor %}
</ul>
{% endfor %}
