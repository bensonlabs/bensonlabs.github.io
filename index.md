title: Fixes
nav_order: 1
Fixes (All)

{% assign fixes = site.pages
| where_exp:"p","p.path contains 'fixes/' and p.name != 'index.md'"
| sort: "title" %}

<ul> {% for p in fixes %} <li><a href="{{ p.url | relative_url }}">{{ p.title }}</a>{% if p.tags %} <small>— {{ p.tags | join: ", " }}</small>{% endif %}</li> {% endfor %} </ul>
