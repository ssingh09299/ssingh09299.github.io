---
layout: page
title:  Academic
permalink: /academic/
---

I accumulate the key points from different sources and write them here;
books are the primary sources for these posts. I am editing the posts as I read
along, if the source is not given it will be updated in time.

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


This is my [Curriculum Vitae]([assets CurriculumVitae Saurabh_curriculum_vitae
pdf](/assets/CurriculumVitae/Saurabh_curriculum_vitae.pdf)).
