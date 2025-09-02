---
layout: home
title: Home
---

## About Me

I am an academic and public policy professional focused on urban policy and governance. My work bridges the gap between rigorous academic research and practical policy implementation in urban settings.

My research examines how cities can develop more effective policies through evidence-based approaches, with particular attention to the intersection of data analytics and public administration.

## Research Focus

**Urban Policy Analysis** - Evaluating the effectiveness of city-level interventions  
**Public Administration** - Studying governance structures in metropolitan areas  
**Policy Implementation** - Bridging theory and practice in urban settings  
**Quantitative Methods** - Applied statistics for policy evaluation

## Recent Publications

{% for item in site.research limit:3 %}
<div class="research-item">
    <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
    {% if item.status %}
        <span class="status-badge status-{{ item.status }}">{{ item.status | replace: '-', ' ' }}</span>
    {% endif %}
    {% if item.authors %}
        <p class="authors">{{ item.authors }}</p>
    {% endif %}
    {% if item.journal and item.year %}
        <p class="publication-info">{{ item.journal }}, {{ item.year }}</p>
    {% endif %}
</div>
{% endfor %}

[View all publications →]({{ '/research/' | relative_url }})

## Current Projects

{% for project in site.projects limit:2 %}
  - [{{ project.title }}]({{ project.url }})
{% endfor %}

*More projects coming soon...*
