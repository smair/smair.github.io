---
layout: page
permalink: /publications/
title: publications
description: 
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2015]
nav: true
nav_order: 2
---

<div class="publications">

{% for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>