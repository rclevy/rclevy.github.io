---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<a href='https://rclevy.github.io/assets/pdf/CV_RLevy_website.pdf'>CV</a> &bull;  <a href='https://ui.adsabs.harvard.edu/public-libraries/y09ZmJBWTfCs0q5KMVKSwQ'>ADS</a> &bull;  <a href='https://orcid.org/0000-0003-2508-2586'>ORCID</a>  &bull; <a href='https://scholar.google.com/citations?user=qXx_t7UAAAAJ&hl=en'>Google Scholar</a>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
