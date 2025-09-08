---
layout: page
title: Projects
permalink: /projects/
---

## Current Projects

{% for project in site.projects %}
<div class="project-item">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    {% if project.status %}
        <span class="status-badge status-{{ project.status }}">{{ project.status | replace: '-', ' ' }}</span>
    {% endif %}
    {% if project.description %}
        <p class="description">{{ project.description }}</p>
    {% endif %}
    {% if project.technologies %}
        <div class="tags">
            {% for tech in project.technologies %}
                <span class="tag">{{ tech }}</span>
            {% endfor %}
        </div>
    {% endif %}
</div>
{% endfor %}

## Past Projects

More projects coming soon...

## Research Software

Information about research tools and software I've developed will be added here.
