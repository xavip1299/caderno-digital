---
layout: page
title: Aulas
permalink: /aulas/
date: 2025-10-17
---

# {{ page.title }}

Resumos e conteúdos das aulas da disciplina Produção de Conteúdos Multimedia.

{% if site.aulas.size > 0 %}
  <div class="collection-list">
    {% for aula in site.aulas %}
      <article class="collection-item">
        <h2><a href="{{ aula.url | relative_url }}">{{ aula.title }}</a></h2>
        {% if aula.date %}
          <p class="item-date">{{ aula.date | date: site.minima.date_format }}</p>
        {% endif %}
        {% if aula.tags %}
          <div class="item-tags">
            {% for tag in aula.tags %}
              <span class="tag">{{ tag }}</span>
            {% endfor %}
          </div>
        {% endif %}
        {% if aula.excerpt %}
          <p class="item-excerpt">{{ aula.excerpt | strip_html | truncatewords: 30 }}</p>
        {% endif %}
      </article>
    {% endfor %}
  </div>
{% else %}
  <p><em>Ainda não há aulas registadas.</em></p>
{% endif %}