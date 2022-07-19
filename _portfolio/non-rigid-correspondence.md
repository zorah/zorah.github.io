---
title: "Non-Rigid Shape Correspondence"
excerpt: "<img width="50%" src='/images/previews/laehner2016elastic2D3D.png'>"
collection: portfolio
---

## Publications

{% for post in site.publications reversed %}
  {% if page.category == 'correspondence' %}
    {% include archive-single-publication.html %}
  {% endif %}
{% endfor %}
