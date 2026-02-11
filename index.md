---
layout: default
title: Opskrifter
---

# Mine opskrifter

## Mad

{% assign recipes = site.pages | where_exp: "p", "p.url contains '.html' and p.url != '/'" | where_exp: "p", "p.url contains '/' and p.dir == '/'" | sort: "title" %}
{% for page in recipes %}
- [{{ page.title }}]({{ page.url | relative_url }})
{% endfor %}

## Drinks

{% assign drinks = site.pages | where_exp: "p", "p.dir == '/Drinks/'" | sort: "title" %}
{% for page in drinks %}
- [{{ page.title }}]({{ page.url | relative_url }})
{% endfor %}
