---
creator: digitalap3
date: 2022-05-02
headerPic: /headers/default-post.jpg
images: [ [ /blog/images/2020/09/olliedino.jpg, 0 ], [ /blog/images/2020/09/olliedreams.jpg, 1 ], [ /blog/images/2020/09/olliehardlife.jpg, 2 ], [ /blog/images/2020/09/ollieflowers.jpg, 3 ], [ /blog/images/2020/09/olliehat.jpg, 4 ], [ /blog/images/2020/09/lowridersleeps.jpg, 5 ] ]
lead: the cutest damn a-hole around with modals
pin: no
postTags: ['Musings', 'Family', 'Test']
slug: 2022/April/gallery-test-with-modal.html
summary: the cutest damn a-hole around with modals
title: Gallery Test with Modal
tags: ['post','images','family','test']

---
## Gallery Test with Modals

<div class="row d-flex justify-content-center">

  {% for imgSrc, daTo in images %}

 <div class="col-12 col-sm-6 col-lg-3">
<img class="img-fluid z-depth-1 border border-info border-4 rounded mt-2 mb-2" src="{{ imgSrc | safe }}" data-bs-toggle="modal" data-bs-target="#modal{{ daTo }}" />
<div class="modal fade" id="modal{{ daTo }}" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
   <div class="modal-content">
   <div class="modal-body mb-0 p-0">
  <img class="img-fluid" src="{{ imgSrc | safe }}" >
  </div>
</div>
</div>
</div>
</div>
  {% endfor %}

</div>

