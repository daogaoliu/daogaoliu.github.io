---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order. The authors of most papers are ordered alphabetically.
years: [2023,2022,2021,2020,2019]
manuyears: [2023,2021]
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


## Manuscript
<div class="publications">

{%- for y in page.manuyears %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f manuscript -q @*[year={{y}}]* %}
{% endfor %}

</div>
