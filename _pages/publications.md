---
layout: page
permalink: /publications/
title: publications
description: Below you will find a list of my current publications. # Enter a description for the "publications" section
years: [2020] # The list of years to divide publications by, e.g., [1967, 1956, 1950, 1935, 1905]
nav: true # Whether (`true`) or not (`false`) to show this section
nav_order: 4 # The order in the navegation bar ("about" is assumed as 0)
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
