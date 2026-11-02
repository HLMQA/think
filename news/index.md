---
layout: page
title: News
---
<div class="news-list">
{% assign items = site.news | sort: "date" | reverse %}
{% for n in items %}
  <p class="news-item"><time>{{ n.date | date: "%-d %b %Y" }}</time><span>{{ n.content | remove: '<p>' | remove: '</p>' | strip }}</span></p>
{% endfor %}
</div>
