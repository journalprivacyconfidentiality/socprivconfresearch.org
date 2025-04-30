---
layout: page
title: SPCR Membership
permalink: /membership/
---

SPCR offers memberships to both [organizations](/organizationalmembers/) and [individuals](/lifetimemembers/), with special options for lifetime membership and students. The information below shows the membership categories and associated benefits.

The membership year is January 1 – December 31.

SPCR is a Section 501(c)(3) nonprofit organization. Membership fees may be deductible for tax purposes; however, we recommend consulting your legal professional or accountant for specific guidance related to your individual tax situation.

To join, click on the appropriate link in the table below.

<table class="display">
  {% for row in site.data.membership %}
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

  <!-- Category,Annual Rate,Benefits,Link Text,Link -->
  <tr>
    <td> {{ row["Category"] }} </td>
    <td> {{ row["Annual Rate"] }} </td>
    <td> {{ row["Benefits"] }} </td>
    <td> <a href="{{ row["Link"] }}" alt="Link to membership fee page">{{ row["Link Text"] }}</a></td>
   </tr>
  {% endfor %}
</table>
