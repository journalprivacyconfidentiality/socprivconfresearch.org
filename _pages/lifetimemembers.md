---
layout: page
title: Lifetime Members SPCR
permalink: /lifetimemembers/
---



<table class="display">
  {% for row in site.data.lifetimemembers %}
    {% if forloop.first %}
    <thead>
    <tr>
      {% for cell in row %}
        {% if forloop.last %}
          {% continue %}
        {% else %}
        <th>{{ cell[0] }}</th>
        {% endif %}
      {% endfor %}
    </tr>
    </thead>
    {% endif %}

  <!-- Member Name,Link,Join Date -->
  <tr>
    <td> <a href="{{ row["Link"] }}" alt="Link to members website">{{ row["Member Name"] }}</a></td>
    <td> {{ row["Join Date"] }}</td>
   </tr>
  {% endfor %}
</table>
