---
layout: page
title: Research
permalink: /research/
menu: true
order: 1
---

## Journal Articles

{% for p in site.data.publications.journal_articles %}
- **{{ p.title }}**,  
  {{ p.journal }} ({{ p.year }})
  vol.{{ p.volume }} {{ p.pages }}. {% if p.coauthors %}(with {{ p.coauthors }}){% endif %}
  {% if p.doi %}
  DOI: {{ p.doi }}
  {% endif %}
{% endfor %}

## Working Papers

{% for p in site.data.publications.working_papers %}
- **{{ p.title }}**,  
  {{ p.media }} ({{ p.year }})
  No.{{ p.number }}. {% if p.coauthors %}(with {{ p.coauthors }}){% endif %}
{% endfor %}

## Presentations

{% for p in site.data.presentations.conference_presentations %}
- **{{ p.title }}**,  
  {{ p.conference }} ({{ p.year }}),
  {{ p.location }} {% if p.coauthors %}(with {{ p.coauthors }}){% endif %}
  {% if p.type %}, {{ p.type }} {% endif %}
{% endfor %}

## Ongoing Projects

- Optimal Funded Pension for Consumers with Heterogeneous Self-Control
- Voluntary provision of durable public goods under present bias and time inconsistency (with Shuichi Tsugawa)
- Resource allocation in repeated contest under present bias (with Shuichi Tsugawa)
