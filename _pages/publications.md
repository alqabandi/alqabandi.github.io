---
layout: page
permalink: /publications/
title: publications 
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">

<h1>journal articles</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1>preprints</h1>

{% bibliography -f preprints %}

{% bibliography %}



</div>
