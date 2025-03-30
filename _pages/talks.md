---
layout: page
permalink: /talks/
title: talks
description: 
nav: true
nav_order: 5
horizontal: false
display_categories: [poster, talk, contributed_talk]
---

<!-- pages/talks.md -->
<div class="talks">
{%- assign talks = site.talks | reverse -%}
<!-- Generate cards for each talk -->
  {%- for talk in talks -%}
    {%- if site.enable_project_categories and page.display_categories %}
    <h2 class="category">{{ talk.category }}</h2>
    {%- endif -%}
    {% include talks.html %}
  {%- endfor %}
</div>

