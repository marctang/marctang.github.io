---
layout: page
permalink: /publications/
title: publications
description:
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

To facilitate identification of author in the literature, I combined my two parent names (Allassonnière and Tang)  starting from 2020. As an overview, since 2017, my publications include {% bibliography_count -f papers --query @article[year >= 2017] %} articles, {% bibliography_count -f papers --query @incollection[year >= 2017] %} book chapters, {% bibliography_count -f papers --query @book[year >= 2017] %} book, and {% bibliography_count -f papers --query @inproceedings[year >= 2017] %} papers in conference proceedings.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
 
</div>

