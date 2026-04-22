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
- {% if p.url %}
      <a href="{{ p.url }}" target="_blank">
        **{{ p.title }}**
      </a>
    {% else %}
      **{{ p.title }}**
    {% endif %} {% if p.coauthors %}(with {{ p.coauthors }}){% endif %},  
  {{ p.media }} ({{ p.year }})
  {% if p.number %}No.{{ p.number }}. {% endif %} 
{% endfor %}

## Presentations

{% for p in site.data.presentations.conference_presentations %}
- **{{ p.title }}** {% if p.coauthors %}(with {{ p.coauthors }}){% endif %},  
  {{ p.conference }} ({{ p.year }}),
  {{ p.location }}
  {% if p.type %}, {{ p.type }} {% endif %}
{% endfor %}

## Ongoing Projects

- Optimal Funded Pension for Consumers with Heterogeneous Self-Control
- Resource allocation in repeated contest under present bias (with Shuichi Tsugawa)
