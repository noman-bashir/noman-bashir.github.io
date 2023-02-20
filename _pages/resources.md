---
layout: table
permalink: /resources/
title: resources
description: A list of relevant conferences. 
nav: true
nav_order: 4
---

{% assign current_module = 0 %}

{% for item in site.data.lectures %}
{% if item.dates %}
{% assign lecture = item %}


<tr>
    <td>
    <div>
        {{ lecture.title }}
    </div>    
    </td>
    <td>
    <div>
        {{ lecture.readings }}
    </div>
    </td>
    <td>
    <div>
        {% if lecture.dates %}
        {% for date in lecture.dates %}
            {{ date }}
        {% endfor %}
        {% endif %}
    </div>
    </td>
</tr>

{% else %}
{% assign current_module = current_module | plus: 1 %}
{% assign module = item %}
<tr class="info">
    <td colspan="5" align="center"><strong><div> {{ module.title }} </div></strong></td>
</tr>
{% endif %}
{% endfor %}
