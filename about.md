---
layout: default
title: About
---
# About page

this is an about page

## images

{% assign image_files = site.static_files | where: "image", true %}
{% for myimage in image_files %}
  {{ myimage.path }}
{% endfor %}