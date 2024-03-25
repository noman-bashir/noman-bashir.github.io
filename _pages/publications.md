---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2015]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<p>Below you can find a list of selected publications including supplementary links.</p>
<p><span class="downloadpdf"><a href="#publications"><i class="fa fa-file-pdf"></i></a>&nbsp;&nbsp;PDF&nbsp;&nbsp;</span>
<span class="downloadpdf"><a href="#publications"><i class="fa fa-file-powerpoint"></i></a>&nbsp;&nbsp;Slides&nbsp;&nbsp;</span>
<span class="download"><a href="#publications"><i class="fa fa-globe"></i></a>&nbsp;&nbsp;Web&nbsp;&nbsp;<a href="#publications"><i class="fa fa-link"></i></a>&nbsp;&nbsp;Bibtex&nbsp;&nbsp;<a href="#publications"><i class="fa fa-code"></i></a>&nbsp;&nbsp;Additional Material</span></p>


{%- for y in page.years %}
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
