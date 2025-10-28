---
title: Fixes
nav_order: 1
---

# Fixes (All)

<ul>
{% for p in site.pages %}
  {% if p.path contains 'fixes/' and p.name != 'index.md' %}
    <li><a href='{{ p.url | relative_url }}'>{{ p.title }}</a>{% if p.tags %} <small>— {{ p.tags | join: ', ' }}</small>{% endif %}</li>
  {% endif %}
{% endfor %}
</ul>