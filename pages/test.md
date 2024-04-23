---
layout: page
title: News and announcements
author: Pradipta Mukherjee
---

# News & Announcements Slideshow

<div id="slideshow-container">
  <div class="slide">
    <h2>New Research Collaboration with XYZ University</h2>
    <p><strong>Posted on April 20, 2024</strong></p>
    <p>We are excited to announce a new research collaboration with XYZ University. This collaboration aims to advance the field of Applied Sciences and foster academic exchange between our institutions.</p>
    <a href="#">Read More</a>
  </div>

  <div class="slide">
    <h2>Upcoming Seminar on Quantum Computing</h2>
    <p><strong>Posted on April 15, 2024</strong></p>
    <p>Don't miss our upcoming seminar on Quantum Computing featuring renowned experts in the field. The seminar will be held on April 30, 2024, at 3:00 PM in the Seminar Hall.</p>
    <a href="#">Register Now</a>
  </div>

  <div class="slide">
    <h2>Call for Papers: International Conference on Applied Sciences</h2>
    <p><strong>Posted on April 10, 2024</strong></p>
    <p>We invite submissions for the International Conference on Applied Sciences to be held on July 20-22, 2024. Submit your research papers by May 31, 2024, for consideration.</p>
    <a href="#">Submit Your Paper</a>
  </div>

  <div class="slide">
    <h2>Scholarship Opportunities for Undergraduate Students</h2>
    <p><strong>Posted on April 5, 2024</strong></p>
    <p>We are pleased to announce scholarship opportunities for undergraduate students pursuing studies in Applied Sciences. Applications are now open until May 15, 2024.</p>
    <a href="#">Apply Now</a>
  </div>

  <div class="slide">
    <h2>Important Update: Changes to Academic Calendar</h2>
    <p><strong>Posted on April 1, 2024</strong></p>
    <p>Please note the following changes to the academic calendar for the current semester. Kindly review the updated schedule to stay informed about important dates and deadlines.</p>
    <a href="#">View Updated Calendar</a>
  </div>
</div>

<script>
  let currentSlide = 0;
  const slides = document.querySelectorAll('.slide');

  function showSlide(index) {
    slides.forEach((slide, i) => {
      if (i === index) {
        slide.style.display = 'block';
      } else {
        slide.style.display = 'none';
      }
    });
  }

  function nextSlide() {
    currentSlide = (currentSlide + 1) % slides.length;
    showSlide(currentSlide);
  }

  setInterval(nextSlide, 5000); // Rotate slides every 5 seconds
  showSlide(currentSlide); // Show initial slide
</script>
