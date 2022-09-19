---
title: "Geometric Deep Learning"
excerpt: "<img width='50%' src='/images/previews/koestler2022intrinsic.png'>"
collection: portfolio
---

## Research Grants

KI-Starter from the Ministry for Culture and Science NRW 'Robust Geometric Deep Learning' (2022-2024) 

## Publications

{% for post in site.publications reversed %}
  {% if post.categories contains 'geometricDL' %}
    {% include archive-single-publication.html %}
  {% endif %}
{% endfor %}
