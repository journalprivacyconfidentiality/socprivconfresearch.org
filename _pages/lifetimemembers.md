---
layout: page
title: Lifetime Members SPCR
permalink: /lifetimemembers/
---

<table class="display">
  <thead>
  <tr><td><em>Name</em></td>
      <td><em>Joined</em></td>
  </tr>
  </thead>
  {% for row in site.data.lifetimemembers %}

  <!-- Member Name,Link,Join Date -->
  <tr>
    <td> <a href="{{ row["Link"] }}" alt="Link to members website">{{ row["Member Name"] }}</a></td>
    <td> {{ row["Join Date"] }}</td>
   </tr>
  {% endfor %}
</table>
