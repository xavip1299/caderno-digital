---
layout: page
title: Projeto Final
permalink: /projeto-final/
date: 2024-10-17
description: "Documentação do projeto final da disciplina"
---

# {{ page.title }}

{% if page.description %}
<p class="page-description">{{ page.description }}</p>
{% endif %}

{% if site.data.disciplina.avaliacao %}
<div class="avaliacao-info">
  <h2>Informação de Avaliação</h2>
  {% for item in site.data.disciplina.avaliacao %}
    {% if item.tipo == "Projeto Final" %}
      <p><strong>Peso:</strong> {{ item.peso }}%</p>
    {% endif %}
  {% endfor %}
</div>
{% endif %}