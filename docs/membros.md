---
title: Membros do PI de Modelagem
site.data.members
---

## Coordenação Geral:
Flora Bacelar

Paulo Inácio Prado
 <ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação Geral e Coordenação das atividades integradoras" %}
        <li>
          <a>
            {{ member.name }}
          </a>
  </li>
      {% endif %}
    {% endfor %}
</ul>

## Coordenação das atividades integradoras:
Charles Santana

Elaine Barbosa

Flora Bacelar

Eduardo Mariano Neto

Gilson Carvalho

Hernane Pereira

Paulo Inácio Prado

Vitor Rios

<ul>
{% for member in site.data.members %}
  <li>
    <a>
      {{ member.name }}
    </a>
    <a>
      {{ member.role }}
    </a>
  </li>
{% endfor %}
</ul>
