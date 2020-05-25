---
layout: page
title: 年终总结
permalink: /summary/
categories: summary
tag: summary
---

{% for category in site.categories %}
  <ul>
    {% if category[0] == page.categories %}
      {% for post in category[1] %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    {% endif %}
  </ul>
{% endfor %}
