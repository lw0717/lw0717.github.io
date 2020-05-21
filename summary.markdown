---
layout: page
title: 年终总结
permalink: /summary/
categories: summary
tag: summary
---

{% for category in site.categories %}
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
