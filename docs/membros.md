---
title: Membros do PI de Modelagem
site.data.members
---
# Membros

...
{% assign membros = site.data.members | group_by: 'role' %}
{% for cat in membros %}
<h2>{{ cat.name }}</h2>
    <ul>
      {% assign items = cat.name %}
      {% for item in items %}
        <li><a href="{{ item.website }}">{{ item.name }}</a></li>
      {% endfor %}
    </ul>
{% endfor %}

...




## Coordenação Geral:
...
<ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação Geral e Coordenação das atividades integradoras"  AND member.status == "ativo" %}
        <li>
          <a>{{ member.name }}<a/>  - {{member.Institution}}
        </li>
      {% endif %}
    {% endfor %}
</ul>
...

## Coordenação das atividades integradoras:

...

<ul>
    {% for member in site.data.members %}
      {% if member.role == "Coordenação das atividades integradoras"  %}
     {% if member.status == "ativo"%}
        <li>
              <a>{{ member.name }}<a/>  - {{member.Institution}}
        </li>
      {% endif %}
      {% endif %}
    {% endfor %}
</ul>

...
## Membros anteriores
...
<ul>
    {% for member in site.data.members %}
      {% if member.status == "inativo" %}
        <li>
          <a>{{ member.name }}<a/>  - {{member.Institution}}
        </li>
      {% endif %}
    {% endfor %}
</ul>
...
