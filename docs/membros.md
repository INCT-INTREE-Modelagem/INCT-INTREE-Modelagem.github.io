---
title: Membros do PI de Modelagem
---

## Coordenação Geral:

<ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação Geral e Coordenação das atividades integradoras"  and member.status == "ativo" %}
    <li>
          <a>{{ member.name }}<a/>  - {{member.Institution}}
    </li>
      {% endif %}
    {% endfor %}
</ul>


## Coordenação das atividades integradoras:
<ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação das atividades integradoras"  %}
        {% if member.status == "ativo" %}
           <li>
              <a>{{ member.name }}<a/>  - {{member.Institution}}
           </li>
        {% endif %}
      {% endif %}
    {% endfor %}
</ul>


## Membros anteriores

<ul>
    {% for member in site.data.members %}
      {% if member.status == "inativo" %}
        <li>
          <a>{{ member.name }}<a/>  - {{member.Institution}}
        </li>
      {% endif %}
    {% endfor %}
</ul>
