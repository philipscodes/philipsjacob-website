---
layout: default
title: "PROFESSIONAL CERTIFICATES"
description: "Philip Jacob - IT Specialist and Programmer"
intro_id: certifications
---
<div class="container-fluid"> <!-- Using container-fluid for full width -->
  <div class="row">
    <!-- Introduction Container -->
      <div class="col-lg-9 col-md-8" >
        {% include intro.html %}
      </div>
    <!-- Tiles Container -->
    <div class="col-lg-3 col-md-4">
      <div class="mt-5">
        {% include tiles.html exclude="Certifications" %}
      </div>
    </div>
  </div>
  <!-- Tiles Container for Certificates -->
  <div class="row">
    <div class="certificate-tiles">
      {% for cert in site.data.certificates %}
        <a href="/certificate_details.html?id={{ cert.id }}">
          <div class="certificate-tile">
            <div class="mt-5">
              <img src="{{ '/images/certificates/' | append: cert.image }}" alt="{{ cert.title }}" style="width: 300px; height: 300px;">
              <p>{{ cert.title }}</p>
            </div>
          </div> 
        </a>
      {% endfor %}
    </div>
  </div>
</div>