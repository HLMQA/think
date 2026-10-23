---
layout: page
title: Publications
---
{% if site.data.publications.size > 0 %}
<ol class="pubs">
  {% for p in site.data.publications %}
  <li><span class="year">{{ p.year }}</span><div><h3>{% if p.url %}<a href="{{ p.url }}">{{ p.title }}</a>{% else %}{{ p.title }}{% endif %}</h3><p>{{ p.authors }}. <em>{{ p.venue }}</em>.</p></div></li>
  {% endfor %}
</ol>
{% else %}
<p class="body muted">Publications will be listed here.</p>
{% endif %}
