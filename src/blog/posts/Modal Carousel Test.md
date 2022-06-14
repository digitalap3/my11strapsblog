---
creator: digitalap3
date: 2022-05-01
headerPic: /headers/default-post.jpg
images: [ [ /blog/images/2020/09/olliedino.jpg, 0, active ], [ /blog/images/2020/09/olliedreams.jpg, 1 ], [ /blog/images/2020/09/olliehardlife.jpg, 2 ], [ /blog/images/2020/09/ollieflowers.jpg, 3 ], [ /blog/images/2020/09/olliehat.jpg, 4 ], [ /blog/images/2020/09/lowridersleeps.jpg, 5 ] ]
lead: testing bootstrap modal carousel
pin: no
postTags: ['Musings', 'Test']
slug: 2022/May/modal-carousel-test.html
summary: testing bootstrap modal carousel
title: Modal Carousel Test
tags: ['post','images','family','test']

---
## Gallery Modal Carousel

This is taking the gallery from [the Gallery Test](/2022/April/gallery-test.html) and turning it into a modal carousel using Booststrap 5. *added active lets see if it works*

<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-hidden="true">
  <div class="modal-dialog" role="document">
   <div class="modal-content">
   <div class="modal-header">
     <button type="button" class="btn-close position-absolute top-5 start-50" data-bs-dismiss="modal" aria-label="Close"></button>
   </div>  
   <div class="modal-body">

   <div id="carouselExample" class="carousel slide" data-bs-interval="false">
   <div class="carousel-inner">

  {% for imgSrc, daTo, active in images %}
   <div class="carousel-item {{ active }}">
   <img class="d-block img-fluid" src="{{ imgSrc | safe }}">
   </div>
 {% endfor %}

   </div>
   </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" style="position: absolute;bottom: 40px; left: 20px;" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
    <span class="carousel-control-next-icon"style="position: absolute;bottom: 40px; right: 20px; aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
   </div>
  </div>
</div>

<div class="row d-flex justify-content-center" id="gallery" data-bs-toggle="modal" data-bs-target="#exampleModal">

  {% for imgSrc, daTo in images %}
  <div class="col-12 col-sm-6 col-lg-3">
   <img class="img-fluid border border-info border-4 rounded mt-2 mb-2" src="{{ imgSrc | safe }}" data-bs-target="#carouselExample" data-bs-slide-to="{{ daTo }}">
  </div>
  {% endfor %}

</div>
