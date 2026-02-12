---
layout: default
title: Opskrifter
---

# Mine opskrifter

{% assign sorted_pages = site.pages | sort: "title" %}

## Hverdagsmad

{% for p in sorted_pages %}{% if p.dir == "/Hverdagsmad/" and p.title %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}

## Bagværk

{% for p in sorted_pages %}{% if p.dir == "/Bagvaerk/" and p.title %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}

## Desserter

{% for p in sorted_pages %}{% if p.dir == "/Desserter/" and p.title %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}

## Drinks

{% for p in sorted_pages %}{% if p.dir == "/Drinks/" and p.title %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}
