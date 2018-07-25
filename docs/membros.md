---
title: Membros do PI de Modelagem
site.data.members
---

## Coordenação Geral:
<ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação Geral e Coordenação das atividades integradoras" %}
        <li>
          <a>{{ member.name }}<a/>  - {{member.Institution}}
        </li>
      {% endif %}
    {% endfor %}
</ul>

## Coordenação das atividades integradoras:
<ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação das atividades integradoras" %}
        <li>
              <a>{{ member.name }}<a/>  - {{member.Institution}}
        </li>
      {% endif %}
    {% endfor %}
</ul>

