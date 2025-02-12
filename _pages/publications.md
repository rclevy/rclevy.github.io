---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2025,2024,2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="social">
  <div class="contact-icons">
    <a href='https://rclevy.github.io/assets/pdf/CV_RLevy_website.pdf' title="CV"><i class="ai ai-cv"></i></a>
    <a href='https://ui.adsabs.harvard.edu/public-libraries/y09ZmJBWTfCs0q5KMVKSwQ' title="ADS"><i class="ai ai-ads"></i></a>
    <a href='https://scixplorer.org/public-libraries/y09ZmJBWTfCs0q5KMVKSwQ' title="SciX"><i class="fas fa-file-alt"></i></a>
    <a href='https://orcid.org/0000-0003-2508-2586' title="ORCID"><i class="ai ai-orcid"></i></a>
    <a href='https://scholar.google.com/citations?user=qXx_t7UAAAAJ&hl=en' title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
  </div>
</div>

<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
