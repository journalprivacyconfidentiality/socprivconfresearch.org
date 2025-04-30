---
layout: listing
title: Donors to SPCR since January 12, 2024
permalink: /donors/
---

<div class="content-section-a">
  <div class="container">

    {% assign donor_types = site.data.donors | map: "Type" | uniq %}
    {% for type in donor_types %}

    <div class="row">
      <div class="col-lg-8">
        <div class="clearfix"></div>
          <a id="{{ type }}" class="anchor-element" aria-label="Donor Type: {{ type }}">
            <h3 class="section-heading">{{ type }}</h3>
          </a>
        
          <table class="display">
            <thead>
              <tr>
                <th>Donor Name</th>
              </tr>
            </thead>
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
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
</div>
