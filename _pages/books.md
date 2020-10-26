---
layout: page
permalink: /books/
title: books
description: books which I read daily and pay much respect to.
years: [1950, 1935, 1905]
nav: true
---

<div class="books">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
