---
layout: default
---
<div class="intro">
  <p>THINK Lab focuses on how interface and interaction design can help users retain cognitive autonomy and independent judgement. Our vision makes human independent judgement a primary design goal, and asks, for each interaction, how to combat mindlessness by design.</p>
  <p class="more"><a href="{{ '/position/' | relative_url }}">Read our position statement</a></p>
</div>

<section class="row">
  <h2>Latest</h2>
  <div>
    {% assign items = site.news | sort: "date" | reverse %}
    {% for n in items limit: 3 %}
      <p class="news-item"><time>{{ n.date | date: "%-d %b %Y" }}</time><span>{{ n.content | remove: '<p>' | remove: '</p>' | strip }}</span></p>
    {% endfor %}
    <p><a class="more" href="{{ '/news/' | relative_url }}">All news</a></p>
  </div>
</section>
