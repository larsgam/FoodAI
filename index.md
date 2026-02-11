---
layout: default
title: Opskrifter
---

# Mine opskrifter

## Mad

{% assign sorted_pages = site.pages | sort: "title" %}
{% for p in sorted_pages %}{% if p.dir == "/" and p.title and p.name != "index.md" %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}

## Drinks

{% for p in sorted_pages %}{% if p.dir == "/Drinks/" and p.title %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}
