---
layout: project
title: Sample Talks
permalink: /talks/
description: A sample of my talks over the years. Not an exhaustive list. 
nav: true
nav_order: 5
display_categories: 
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

    <div class="row row-cols-1 row-cols-md-2">
        {% for project in sorted_projects %}
        {% include projects.liquid %}
        {% endfor %}
    </div>
</div>