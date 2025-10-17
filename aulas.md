---
layout: page
title: Aulas
permalink: /aulas/
date: 2024-10-17
---

# {{ page.title }}

{% if site.collections.aulas.docs.size > 0 %}
  <div class="collection-list">
    {% for aula in site.aulas %}
      <div class="collection-item">
        <h3><a href="{{ aula.url | relative_url }}">{{ aula.title }}</a></h3>
        {% if aula.date %}
          <p class="item-date">{{ aula.date | date: site.minima.date_format }}</p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
{% else %}
  <p><em>Ainda não há aulas registadas.</em></p>
{% endif %}