---
layout: page
permalink: /publications/
title: Publications
description:
years: [In press, Under review, 2024, 2023, 2022, 2021, 2020, 2019, 2017]
patentyears: [Granted]
nav: true
---
<!-- _pages/publications.md -->

<div class="publications">

More information can be found at <a href="https://scholar.google.com/citations?user=9PY80DQAAAAJ">Google Scholar</a>

<br>

† denotes equal contribution | * denotes corresponding authorship

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

---

### Patents

<div class="publications">

{%- for y in page.patentyears %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>
