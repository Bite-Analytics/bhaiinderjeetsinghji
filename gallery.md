
---
layout: single
title: "Gallery"
excerpt: "Photos from the life and journey of Bhai Inderjeet Singh Ji."
permalink: /gallery/
author_profile: true
---

<style>
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  gap: 12px;
  margin: 2rem 0;
}
.gallery-grid img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
  cursor: pointer;
  transition: transform 0.2s ease;
}
.gallery-grid img:hover {
  transform: scale(1.03);
}
.lightbox {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.85);
  z-index: 999;
  align-items: center;
  justify-content: center;
}
.lightbox:target {
  display: flex;
}
.lightbox img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 6px;
}
.lightbox-close {
  position: absolute;
  top: 20px;
  right: 30px;
  color: white;
  font-size: 2.5rem;
  text-decoration: none;
  line-height: 1;
}
</style>

<!-- THUMBNAILS: one <a><img></a> per photo. href="#imgN" must match the id="imgN" of its lightbox block below. -->
<div class="gallery-grid">
  <a href="#img1"><img src="/images/gallery/photo1.jpg" alt="Gallery photo 1"></a>
  <a href="#img2"><img src="/images/gallery/photo2.jpg" alt="Gallery photo 2"></a>
</div>

<!-- LIGHTBOXES: one block per photo, id must match the thumbnail's href above. -->
<div id="img1" class="lightbox">
  <a href="#" class="lightbox-close">&times;</a>
  <img src="/images/gallery/Photo1.jpg" alt="Gallery photo 1">
</div>

<div id="img2" class="lightbox">
  <a href="#" class="lightbox-close">&times;</a>
  <img src="/images/gallery/Photo2.jpg" alt="Gallery photo 2">
</div>

<!--
  TO ADD A NEW PHOTO (e.g. photo3.jpg):
  1. Upload photo3.jpg to /images/gallery/
  2. Add this thumbnail inside the <div class="gallery-grid"> block above:
       <a href="#img3"><img src="/images/gallery/photo3.jpg" alt="Gallery photo 3"></a>
  3. Add this lightbox block down here, after the last one:
       <div id="img3" class="lightbox">
         <a href="#" class="lightbox-close">&times;</a>
         <img src="/images/gallery/photo3.jpg" alt="Gallery photo 3">
       </div>
  4. Repeat with img4/photo4.jpg, img5/photo5.jpg, etc.
-->
