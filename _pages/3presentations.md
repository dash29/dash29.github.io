---
layout: page
permalink: /presentations/
title: presentations
description:
years: [2020, 2019]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}
