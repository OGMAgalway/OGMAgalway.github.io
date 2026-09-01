---
layout: default
title: O G M A
---

<style>
/* Slideshow container */
.slideshow-container {
    max-width: 800px;
    position: relative;
    margin: auto;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.5);
}

/* Hide all slides by default */
.mySlides {
    display: none;
    width: 100%;
}

/* Fading animation */
.fade {
    animation-name: fade;
    animation-duration: 1.5s;
}

@keyframes fade {
    from {opacity: 0.4}
    to {opacity: 1}
}

/* Make images responsive */
.mySlides img {
    width: 100%;
    height: auto;
    display: block;
}

/* Caption text */
.text {
    color: #f2f2f2;
    font-size: 20px;
    padding: 8px 12px;
    position: absolute;
    bottom: 8px;
    width: 100%;
    text-align: center;
    background: rgba(0,0,0,0.6);
    box-sizing: border-box;
}
</style>

# O G M A

Traditional Irish music from the Wild Atlantic Way

## Slideshow

<div class="slideshow-container">

    <!-- Slide 1 -->
    <div class="mySlides fade">
        <img src="/images/ogma1.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 2 -->
    <div class="mySlides fade">
        <img src="/images/ogmaA3.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 3 -->
    <div class="mySlides fade">
        <img src="/images/ogmaA2.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

</div>

## Listen

[Add your Spotify or Bandcamp link]

## Upcoming Shows

- Friday, June 15 - Club Venue, City
- Saturday, June 16 - Bar Lounge, Town

## Contact

[opentrad@yahoo.com]

<script>
    let slideIndex = 0;
    showSlides();

    function showSlides() {
        let slides = document.getElementsByClassName("mySlides");
        
        // Hide all slides
        for (let i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
        }
        
        // Move to the next slide
        slideIndex++;
        if (slideIndex > slides.length) { slideIndex = 1; }
        
        // Show the current slide
        slides[slideIndex - 1].style.display = "block";
        
        // Change image every 4 seconds (4000ms)
        setTimeout(showSlides, 4000);
    }
</script>
