---
layout: page
title:  Academic
permalink: /academic/
---

{% highlight python %}
# This is a python snippet
import numpy as np
a = np.array([1, 2, 3, 4])
{% endhighlight %}

This is working.


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
