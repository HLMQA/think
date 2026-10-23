---
layout: page
title: People
---
{% for group in site.data.people %}
<section class="row">
  <h2>{{ group.group }}</h2>
  <div class="people">
    {% for p in group.members %}
    <article class="person">
      {% if p.photo %}<img class="photo" src="{{ '/assets/img/' | append: p.photo | relative_url }}" alt="{{ p.name }}">{% endif %}
      <div>
        <h3>{{ p.name }}</h3>
        {% if p.role %}<p class="role">{{ p.role }}</p>{% endif %}
        <p class="body">{{ p.bio }}</p>
      </div>
    </article>
    {% endfor %}
  </div>
</section>
{% endfor %}
