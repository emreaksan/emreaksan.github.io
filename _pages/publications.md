---
layout: page
permalink: /publications/
title: Publications
description: 

years: [2022, 2021, 2020, 2019, 2018, 2017, 2015]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
<span>An up-to-date list is available at <a href="https://scholar.google.com/citations?user=0P_684sAAAAJ&hl=en" color="#a31f34" target="_blank" rel="noopener noreferrer">Google Scholar</a>.</span>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
