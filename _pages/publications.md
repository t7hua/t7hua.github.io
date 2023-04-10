---
layout: page
permalink: /publications/
title: Publications 
description: '*' indicates equal contribution. <u><a href='https://scholar.google.com/citations?user=ynA-x2wAAAAJ&hl'>Google Scholar</a></u> contains a more complete list of my publications.
years: [2022, 2021, 2020, 2018, 2016, 2014, 2013]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>