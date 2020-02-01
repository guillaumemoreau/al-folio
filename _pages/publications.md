---
layout: page
permalink: /publications/
title: Recent publications
description: Publications for the last 3 years
years: [2019, 2018, 2017]
---

Other lists:

  - sorted by type:
  - [sorted by year](../allpubyear/)


{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
