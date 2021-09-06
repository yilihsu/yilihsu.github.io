---
layout: page
permalink: /publications/
title: Publications
description: In reversed chronological order.
years: [2021, 2020, 2019, 2016, 2015, 2014, 2013]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
