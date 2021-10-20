---
layout: page
permalink: /publications/
title: publications
description:
years: [2021, 2020, 2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <div class="row">
    <div class="col-sm-12">
      <h2 class="year">{{y}}</h2>
    </div>
  </div>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>