---
layout: default
---
<div class="intro">
  <p>think lab studies how interfaces shape the way we interpret. AI systems and visualisations both present interpretation as fact. We design interfaces that ask people to <em>think</em> instead.</p>
</div>

<section class="row">
  <h2>Latest</h2>
  <div>
    {% assign items = site.news | sort: "date" | reverse %}
    {% for n in items limit: 3 %}
      <p class="news-item"><time>{{ n.date | date: "%-d %b %Y" }}</time>{{ n.content | strip_html | strip }}</p>
    {% endfor %}
    <p><a class="more" href="{{ '/news/' | relative_url }}">All news</a></p>
  </div>
</section>
