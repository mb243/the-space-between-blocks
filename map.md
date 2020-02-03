---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: map
layout: default
---

![Biome Map](images/biomes_3.png)

_Click [here](images/biome_key.png) to view the biome color key._

The following user-contributed points of interest are sourced from [overworld.csv](overworld.csv):

<table>
{% for row in site.data.overworld %}
  <tr>
      <td> <strong>
      {% if row.href != nil %}<a href="{{ row.href }}">{% endif %}
      {{ row.Description }}
      {% if row.href != nil %}</a>{% endif %}
      </strong> </td> <td> {{ row.x }} </td> <td> {{ row.z }} </td>
  </tr>
{% endfor %}
</table>