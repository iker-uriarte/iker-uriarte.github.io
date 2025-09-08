---
layout: page
title: Curriculum Vitae
permalink: /cv/
---

*Full CV available upon request*

## Education

<div class="cv-entry">
    <div class="cv-title">Ph.D. in Political and Social Science</div>
    <div class="cv-organization">Pompeu Fabra University</div>
    <div class="cv-date">Expected 2026</div>
    <p>Dissertation: "Three Essays on Democratic Policy Implementation"</p>
</div>

<div class="cv-entry">
    <div class="cv-title">M.Sc. in Political and Electoral Analysis</div>
    <div class="cv-organization">University Carlos III - Juan March Institute</div>
    <div class="cv-date">2021</div>
</div>

<div class="cv-entry">
    <div class="cv-title">B.A. in Sociology</div>
    <div class="cv-organization">University of Salamanca</div>
    <div class="cv-date">2019</div>
</div>

## Professional Experience

<div class="cv-entry">
    <div class="cv-title">Editorial Assistant</div>
    <div class="cv-organization">Journal of Public Policy</div>
    <div class="cv-date">2023 - Present</div>
    <p>Supported public communications by managing social media channels, crafting engaging content to highlight key publications, and coordinating outreach strategies to increase visibility and readership</p>
</div>

<div class="cv-entry">
    <div class="cv-title">Pre Doctoral Fellow, REPGOV project (ERC funded)</div>
    <div class="cv-organization">Institut Barcelona d'Estudis Internacionals</div>
    <div class="cv-date">2022 - Present</div>
    <p>Contributed to research on caretaker governments and legislative politics through large-scale data collection, systematic literature reviews, and quantitative analysis of lawmaking processes in Spain and Italy.</p>
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
