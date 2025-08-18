---
layout: page
title: Organizational Members SPCR
permalink: /organizationalmembers/
---



<table class="display">
  {% for row in site.data.organizationalmembers %}
    {% if forloop.first %}
    <thead>
    <tr>
      <th>Member</th>
      <th>Joined</th>
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
