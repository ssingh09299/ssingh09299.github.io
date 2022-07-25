---
layout: page
title:  Research
permalink: /research/
---

I write about a selected set of my research areas here. Currently, I am working on inter-particle interaction of granular particles (sands, ballasts, etc.).


{% for category in site.categories %}
{% if category[0] == "Force chains" %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}

{% for category in site.categories %}
{% if category[0] == "X-ray CT for soils" %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}

## Important links

1. [Segmentation of three-dimensional X-ray computed tomography scans of granular materials using Morse theory](https://bitbucket.org/vgl_iisc/morsegram)
2. [Segmentation of three-dimensional X-ray computed tomography scans of granular materials using Watershed algorithm](https://github.com/ssingh09299/SandLabs)
3. [Integration of Lade's constitutive model](https://github.com/ssingh09299/Lade-Model)
4. [Particle image velocimetry for beginners](https://github.com/ssingh09299/Particle-Image-Velocimetry)
