---
layout: page
title: 投资小记
permalink: /investment/
categories: investment
tag: investment
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
