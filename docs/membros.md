---
title: Membros do PI de Modelagem
site.data.members
---

## Coordenação Geral:
Flora Bacelar

Paulo Inácio Prado

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
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>
