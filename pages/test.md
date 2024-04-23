---
layout: page
title: News and announcements
author: Pradipta Mukherjee
---

# Cycling Slideshow of Images with Links

<div id="slideshow">
  <img class="slide" src="https://via.placeholder.com/200" alt="Image 1 Description">
  <img class="slide" src="https://via.placeholder.com/200" alt="Image 2 Description">
  <img class="slide" src="https://via.placeholder.com/200" alt="Image 3 Description">
  <img class="slide" src="https://via.placeholder.com/200" alt="Image 4 Description">
  <img class="slide" src="https://via.placeholder.com/200" alt="Image 5 Description">
</div>

<div id="links">
  <a id="link1" href="https://octresearch.org/research/">Visit Website 1</a>
  <a id="link2" href="https://cbme.iitd.ac.in/faculty">Visit Website 2</a>
  <a id="link3" href="https://cbme.iitd.ac.in">Visit Website 3</a>
  <a id="link4" href="https://cbme.iitd.ac.in/about">Visit Website 4</a>
  <a id="link5" href="https://cbme.iitd.ac.in/ongoing-research">Visit Website 5</a>
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

  function rotateSlides() {
    currentIndex = (currentIndex + 1) % slides.length;
    showSlide(currentIndex);
  }

  setInterval(rotateSlides, 5000); // Rotate slides every 5 seconds
</script>
