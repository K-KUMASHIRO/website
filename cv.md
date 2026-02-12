---
layout: page
title: CV
permalink: /cv/
menu: true
order: 3
---

## Education
{% for item in site.data.cv.education %}
- {{ item.year }}: {{ item.detail }}
{% endfor %}

## Academic Positions
{% for item in site.data.cv.positions %}
- {{ item.year }}: {{ item.detail }}
{% endfor %}
