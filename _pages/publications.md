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

<p>Below, you can find a list of <strong>selected publications</strong>, including supplementary links. In almost all of my publications, the author names are in the following order: 

<ul>
  <li>Ph.D. students in the order of their contributions.</li>
  <li>Postdocs in the order of their contributions.</li>
  <li>Faculty members in the order of their contribution.</li>
</ul>


Often, the first author's advisor goes last in the authorship order, but this rule is loosely followed.</p>
<p></p>

<p><span class="downloadpdf"><a href="#publications"><i class="fa fa-file-pdf"></i></a>&nbsp;&nbsp;PDF&nbsp;&nbsp;</span>
<span class="downloadpdf"><a href="#publications"><i class="fa fa-file-powerpoint"></i></a>&nbsp;&nbsp;Slides&nbsp;&nbsp;</span>
<span class="download"><a href="#publications"><i class="fa fa-globe"></i></a>&nbsp;&nbsp;Web&nbsp;&nbsp;<a href="#publications"><i class="fa fa-link"></i></a>&nbsp;&nbsp;Bibtex&nbsp;&nbsp;<a href="#publications"><i class="fa fa-code"></i></a>&nbsp;&nbsp;Additional Material</span></p>


{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
