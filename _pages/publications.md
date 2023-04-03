---
layout: page
permalink: /publications/
title: publications
description: Conference proceedings, workshop papers, journal papers, etc. <u><a href='https://scholar.google.com/citations?user=ynA-x2wAAAAJ&hl'>Google Scholar</a></u> contains a more complete list of my publications.
years: [2018, 2020, 2021, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>