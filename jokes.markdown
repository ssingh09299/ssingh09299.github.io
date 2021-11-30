---
layout: page
title:  Jokes
permalink: /jokes/
---

Enjoy reading the following:

{% for category in site.categories %}
{% if category[0] == "Jokes" %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}
