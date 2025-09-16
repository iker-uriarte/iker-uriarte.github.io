---
layout: home
title: Home
---

## About Me

I am a PhD candidate in Political and Social Sciences at Universitat Pompeu Fabra and a pre-doctoral fellow at the Institut Barcelona d’Estudis Internacionals (IBEI). My research examines how democratic and bureaucratic accountability collide in practice, with a focus on participatory processes and governance in cities such as New York City and Barcelona. Along the way, I use quantitative methods to make sense of how institutions try (and often fail) to deliver on their promises.

In addition to my academic work, I am passionate about fostering collaboration between scholars, policymakers, and local communities. I believe that meaningful change emerges when research is accessible and actionable, and I strive to bridge the gap between theory and practice through public engagement and interdisciplinary partnerships. My experiences in both New York and Barcelona have shaped my commitment to inclusive governance and evidence-based policy, and I am dedicated to transforming the way we understand democratic practices and reimagining our institutions for a more inclusive and equal society. Outside of academia, I’m a fairly competent bass player and a film enthusiast—hit me up if that’s your jam too, I’m always happy to talk about music or movies.

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
