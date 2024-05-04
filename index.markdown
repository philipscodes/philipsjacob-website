---
layout: default
title: "WELCOME TO MY WEBSITE"
description: "Philip Jacob - IT Specialist and Programmer"
intro_id: home
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
        {% include tiles.html exclude="Home" %}
      </div>
    </div>
  </div>
</div>