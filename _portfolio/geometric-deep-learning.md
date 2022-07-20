---
title: "Geometric Deep Learning"
excerpt: "<img width='50%' src='/images/previews/laehner2016elastic2D3D.png'>"
collection: portfolio
---

This is a test.

## Publications

{% for post in site.publications reversed %}
  {% if post.categories contains 'correspondence' %}
    {% include archive-single-publication.html %}
  {% endif %}
{% endfor %}
