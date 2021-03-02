---
layout: page
title: Personal
permalink: /personal/
---




{% for category in site.categories %}
{% if category[0] == "Personal Writings" %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}

