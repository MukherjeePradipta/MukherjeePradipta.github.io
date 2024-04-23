---
layout: page
title: News and announcements
author: Pradipta Mukherjee
---

# Cycling Slideshow of Images with Links

<div id="slideshow">
  <img class="slide" src="image1.jpg" alt="Image 1 Description">
  <img class="slide" src="image2.jpg" alt="Image 2 Description">
  <img class="slide" src="image3.jpg" alt="Image 3 Description">
  <img class="slide" src="image4.jpg" alt="Image 4 Description">
  <img class="slide" src="image5.jpg" alt="Image 5 Description">
</div>

<div id="links">
  <a id="link1" href="http://www.website1.com">Visit Website 1</a>
  <a id="link2" href="http://www.website2.com">Visit Website 2</a>
  <a id="link3" href="http://www.website3.com">Visit Website 3</a>
  <a id="link4" href="http://www.website4.com">Visit Website 4</a>
  <a id="link5" href="http://www.website5.com">Visit Website 5</a>
</div>

<script>
  let currentIndex = 0;
  const slides = document.querySelectorAll('.slide');
  const links = document.querySelectorAll('#links a');

  function showSlide(index) {
    slides.forEach((slide, i) => {
      if (i === index) {
        slide.style.display = 'block';
      } else {
        slide.style.display = 'none';
      }
    });
    
    links.forEach((link, i) => {
      if (i === index) {
        link.style.display = 'inline';
      } else {
        link.style.display = 'none';
      }
    });
  }

  function nextSlide() {
    currentIndex = (currentIndex + 1) % slides.length;
    showSlide(currentIndex);
  }

  setInterval(nextSlide, 5000); // Change slide every 5 seconds
  showSlide(currentIndex); // Show initial slide
</script>
