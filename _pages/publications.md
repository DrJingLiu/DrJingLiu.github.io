---
layout: page
permalink: /publications/
title: Publications
description: Publications by years in reversed chronological order.
years: [2022,2021,2020,2019,2017,2016,2012]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year"><font color="grey">{{y}}</font></h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
