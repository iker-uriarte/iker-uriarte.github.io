---
layout: default
title: Home
---

# Welcome

I am an academic and public policy professional interested in [your research areas]. My work bridges the gap between academic research and practical policy implementation.

## Research Interests

- Interest 1
- Interest 2
- Interest 3

## Recent Publications

{% for item in site.research limit:3 %}
  - [{{ item.title }}]({{ item.url }})
{% endfor %}

## Current Projects

{% for project in site.projects limit:3 %}
  - [{{ project.title }}]({{ project.url }})
{% endfor %}

## Contact

Feel free to reach out at [your email] or connect with me on [LinkedIn/Twitter/etc].
