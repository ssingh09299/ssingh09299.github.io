---
layout: page
title: Personal
permalink: /personal/
---

I express myself here--about life, ideas, and experiences. These are modified
time to time, and may appear incomplete at times.

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

