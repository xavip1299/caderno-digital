---
layout: page
title: Exercícios Práticos  
permalink: /exercicios/
date: 2025-10-17
---

# {{ page.title }}

{% if site.collections.exercicios.docs.size > 0 %}
  <div class="collection-list">
    {% for exercicio in site.exercicios %}
      <div class="collection-item">
        <h3><a href="{{ exercicio.url | relative_url }}">{{ exercicio.title }}</a></h3>
        {% if exercicio.date %}
          <p class="item-date">{{ exercicio.date | date: site.minima.date_format }}</p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
{% else %}
  <p><em>Ainda não há exercícios registados.</em></p>
{% endif %}