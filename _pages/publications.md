---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---

<details>
<summary>Preprints</summary>
<div class="publications">

{% for y in page.years %}
  {% bibliography -f preprint -q @*[year={{y}}]* %}
{% endfor %}

</div>
</details>

##### Books

<div class="publications">

{% for y in page.years %}
  {% bibliography -f books -q @*[year={{y}}]* %}
{% endfor %}

</div>

##### Papers

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f pubs -q @*[year={{y}}]* %}
{% endfor %}

</div>
