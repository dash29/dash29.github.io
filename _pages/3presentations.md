---
layout: page
permalink: /presentations/
title: presentations
description:
years: [2019, 2020]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}
