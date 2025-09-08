---
layout: page
title: Research
permalink: /research/
---

## Publications

{% for paper in site.research %}
<div class="research-item">
    <h3><a href="{{ paper.url }}">{{ paper.title }}</a></h3>
    {% if paper.status %}
        <span class="status-badge status-{{ paper.status }}">{{ paper.status | replace: '-', ' ' }}</span>
    {% endif %}
    {% if paper.authors %}
        <p class="authors">{{ paper.authors }}</p>
    {% endif %}
    {% if paper.journal and paper.year %}
        <p class="publication-info">{{ paper.journal }}, {{ paper.year }}</p>
    {% endif %}
    {% if paper.abstract %}
        <p class="abstract">{{ paper.abstract | truncate: 200 }}</p>
    {% endif %}
    {% if paper.tags %}
        <div class="tags">
            {% for tag in paper.tags %}
                <span class="tag">{{ tag }}</span>
            {% endfor %}
        </div>
    {% endif %}
</div>
{% endfor %}

## Working Papers

Coming soon...

## Research Interests

- Public policy analysis
- Quantitative methods in social science
- Policy evaluation and impact assessment
