---
layout: page
title: Curriculum Vitae
permalink: /cv/
---

## Education

<div class="cv-entry">
    <div class="cv-title">Ph.D. in Public Policy</div>
    <div class="cv-organization">University Name</div>
    <div class="cv-date">Expected 2025</div>
    <p>Dissertation: "Title of Your Dissertation"</p>
</div>

<div class="cv-entry">
    <div class="cv-title">M.A. in Public Administration</div>
    <div class="cv-organization">University Name</div>
    <div class="cv-date">2020</div>
</div>

## Professional Experience

<div class="cv-entry">
    <div class="cv-title">Policy Analyst</div>
    <div class="cv-organization">Organization Name</div>
    <div class="cv-date">2021 - Present</div>
    <p>Brief description of your role and key accomplishments.</p>
</div>

## Publications

### Peer-Reviewed Articles

{% for paper in site.research %}
<div class="cv-entry">
    <div class="cv-title">{{ paper.title }}</div>
    {% if paper.authors %}<div class="cv-organization">{{ paper.authors }}</div>{% endif %}
    {% if paper.journal and paper.year %}<div class="cv-date">{{ paper.journal }}, {{ paper.year }}</div>{% endif %}
</div>
{% endfor %}

## Research Interests

- Policy evaluation and impact assessment
- Quantitative methods in social science
- Public administration and governance
- Evidence-based policymaking

## Skills

**Statistical Software:** R, Stata, SPSS, Python  
**Other:** GIS, Qualitative data analysis, Survey design

---

*Last updated: {{ site.time | date: '%B %Y' }}*
