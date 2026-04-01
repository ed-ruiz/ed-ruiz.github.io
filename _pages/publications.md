---
layout: page
permalink: /publications/
title: publications
description: Publications and technical reports
years: [2025, 2020, 2019, 2018, 2016, 2014]
nav: true
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
