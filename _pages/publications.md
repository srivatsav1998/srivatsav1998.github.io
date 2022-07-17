---
layout: page
permalink: /publications/
title: publications
description: List of my publications in reversed chronological order. Also, check my <a href='https://scholar.google.com/citations?user=DWSiIooAAAAJ&hl=en'>Google Scholar</a>.
years: [2021, 2020]
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
