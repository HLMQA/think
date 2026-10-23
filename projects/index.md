---
layout: page
title: Projects
---
<div class="cards">
  {% assign items = site.projects | sort: "order" %}
  {% for p in items %}
  <article>
    <h3><a href="{{ p.url | relative_url }}">{{ p.title }}</a></h3>
    <p>{{ p.summary }}</p>
  </article>
  {% endfor %}
</div>
