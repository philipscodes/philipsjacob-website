---
layout: default
title: "INTERVIEW VIDEOS"
description: "Philip Jacob - IT Specialist and Programmer"
intro_id: videos
---
<div class="container-fluid"> <!-- Using container-fluid for full width -->
  <div class="row">
    <!-- Introduction Container -->
    <div class="col-lg-9 col-md-8">
      {% include intro.html %}
    </div>
    <!-- Tiles Container -->
    <div class="col-lg-3 col-md-4">
      <div class="mt-5">
        {% include tiles.html exclude="Videos" %}
      </div>
    </div>
  </div>
  <!-- Video Thumbnails Container -->
  <div class="row">
    <div class="col-sm-12">
      <div class="video-container mt-4">    
        <div class="row">
          {% for video in site.data.videos %}  
            <div class="col-md-4 mb-4">
              <a href="https://www.youtube.com/watch?v={{ video.id }}" class="card-link" target="_blank">
                <div class="card">
                  <img src="https://img.youtube.com/vi/{{ video.id }}/0.jpg" class="card-img-top img-fluid" alt="{{ video.title }}">
                    <div class="card-body">
                      <h5 class="card-title">{{ video.title }}</h5>
                    </div>
                </div>
              </a>  
            </div>
          {% endfor %}  
        </div>
      </div>
    </div>  
  </div>  
</div>