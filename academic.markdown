---
layout: page
title:  Academic
permalink: /academic/
---

Here I post my academic writings.


{% for category in site.categories %}
{% if category[0] == "Academic Writings" %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}


This is my [Curriculum
Vitae](/assets/CurriculumVitae/Saurabh_curriculum_vitae.pdf).
