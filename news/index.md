---
layout: page
title: News
---
<div class="news-list">
{% assign items = site.news | sort: "date" | reverse %}
{% for n in items %}
  <p class="news-item"><time>{{ n.date | date: "%-d %b %Y" }}</time>{{ n.content | strip_html | strip }}</p>
{% endfor %}
</div>
