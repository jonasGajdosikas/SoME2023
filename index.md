---
title: Home
layout: default
---

<h1 style="text-align:center">Dice and Calculators and Simplex numbers</h1>

> How I discovered discovering math


{% assign revposts = site.posts | reverse %}
{% for item in revposts %}
<h4><a href="{{ item.url | relative_url }}">
    {{ item.title }}
</a></h4>
{% endfor %}

