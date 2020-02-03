---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: map
layout: default
---

![Biome Map](images/biomes_3.png)

_Click [here](images/biome_key.png) to view the biome color key._

# Points of Interest

The following are user-contributed points of interest:

## [The Overworld](overworld.csv):
<table>
<tr><th>Description</th><th>x</th><th>z</th></tr>
{% for row in site.data.overworld %}
  <tr>
      <td>
      {% if row.href != nil %}<a href="{{ row.href }}">{% endif %}
      {{ row.Description }}
      {% if row.href != nil %}</a>{% endif %}
      </td> <td> {{ row.x }} </td> <td> {{ row.z }} </td>
  </tr>
{% endfor %}
</table>

## [The Nether](nether.csv):
<table>
<tr><th>Description</th><th>x</th><th>z</th></tr>
{% for row in site.data.nether %}
  <tr>
      <td>
      {% if row.href != nil %}<a href="{{ row.href }}">{% endif %}
      {{ row.Description }}
      {% if row.href != nil %}</a>{% endif %}
      </td> <td> {{ row.x }} </td> <td> {{ row.z }} </td>
  </tr>
{% endfor %}
</table>

## [The End](end.csv):
<table>
<tr><th>Description</th><th>x</th><th>z</th></tr>
{% for row in site.data.end %}
  <tr>
      <td>
      {% if row.href != nil %}<a href="{{ row.href }}">{% endif %}
      {{ row.Description }}
      {% if row.href != nil %}</a>{% endif %}
      </td> <td> {{ row.x }} </td> <td> {{ row.z }} </td>
  </tr>
{% endfor %}
</table>
