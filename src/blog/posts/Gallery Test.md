---
creator: digitalap3
date: 2022-05-09
headerPic: /headers/default-post.jpg
images: [ [ /blog/images/2020/09/olliedino.jpg, 0 ], [ /blog/images/2020/09/olliedreams.jpg, 1 ], [ /blog/images/2020/09/olliehardlife.jpg, 2 ], [ /blog/images/2020/09/ollieflowers.jpg, 3 ], [ /blog/images/2020/09/olliehat.jpg, 4 ], [ /blog/images/2020/09/lowridersleeps.jpg, 5 ] ]
lead: 
pin: no
postTags: ['musings', 'family']
slug: 2022/April/gallery-test.html
summary: the cutest damn a-hole around
title: Gallery Test
tags: ['post', 'family', 'images']

---
## Gallery Test

<div class="row d-flex justify-content-center" id="gallery">

  {% for imgSrc, daTo in images %}
  <div class="col-12 col-sm-6 col-lg-3">
          <img class="w-100 border border-info border-4 rounded mt-2 mb-2" src="{{ imgSrc | safe }}">
  </div>
  {% endfor %}

</div>
