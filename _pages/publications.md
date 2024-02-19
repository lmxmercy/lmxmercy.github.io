---
layout: page
permalink: /publications/
title: publications
description: "* indicates equal contribution."
years: [2022, 2021, 2020, 2019, 2016, 2015, 2014, 2012, 2011]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

