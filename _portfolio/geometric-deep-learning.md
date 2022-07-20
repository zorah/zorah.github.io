---
title: "Geometric Deep Learning"
excerpt: "<img width='50%' src='/images/previews/koestler2022intrinsic.png'>"
collection: portfolio
---

This is a test.

## Publications

{% for post in site.publications reversed %}
  {% if post.categories contains 'geometricDL' %}
    {% include archive-single-publication.html %}
  {% endif %}
{% endfor %}
