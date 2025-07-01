---
layout: page
title: Donations and Donors 
permalink: /donors/
---

  
To make a donation to SPCR, please visit our [donation page](https://www.zeffy.com/donation-form/donate-to-spcr).

<h3>Donors to SPCR since January 12, 2024</h3>

{% assign donor_types = site.data.donors | map: "Type" | uniq %}
{% for type in donor_types %}


    
<a id="{{ type }}" class="anchor-element" aria-label="Donor Type: {{ type }}"></a>
<h4 class="section-heading">{{ type }}</h4>


<table class="display">
  
  <tbody>
    {% for row in site.data.donors %}
      {% if row["Type"] == type %}
      <tr>
        <td>{{ row["Donor Name"] }}</td>
      </tr>
      {% endif %}
    {% endfor %}
  </tbody>
</table>
<br/>
{% endfor %}