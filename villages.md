---
title: Villages
layout: default
---
# Villages 

This is a player-provided list of villages and villager trades. Both natural villages and player-built trading halls can be listed here. Data is sourced from villages.yml.

{% for village in site.data.villages %}
## {{ village.heading }}

**Description**: {{ village.description }}<br/>
**Location**: X: {{ village.x }} / Y: {{ village.y }}

**Trades available here**:

<table>
    {% for item in village.trades %}
        <tr>
        <td style="width:50%;">{{ item[0] }}</td>
        <td style="width:50%;">{{ item[1] }}</td>
        </tr>
    {% endfor %}
</table>
{% endfor %}