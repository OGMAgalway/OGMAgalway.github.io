---
layout: default
title: 
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

/* Smooth fade transition */
.fade {
    animation-name: fade;
    animation-duration: 2s; /* Slower fade for smoother transition */
}

@keyframes fade {
    0% { opacity: 0; }
    20% { opacity: 1; } /* Holds at full opacity longer */
    80% { opacity: 1; } /* Holds at full opacity longer */
    100% { opacity: 0; }
}

/* Combined Fade + Zoom */
.fade-zoom {
    animation: fadeZoom 2s ease-in-out;
}

@keyframes fadeZoom {
    0% { 
        opacity: 0; 
        transform: scale(0.85); 
    }
    50% { 
        opacity: 1; 
        transform: scale(1.55); 
    }
    100% { 
        opacity: 1; 
        transform: scale(1); 
    }
}

@keyframes zoomBase {
    0% { transform: scale(1); }
    25% { transform: scale(1); }
    75% { transform: scale(1.95); }
    100% { transform: scale(1.95); }
}

/* Different zoom origins */
.zoom-center {
    animation: zoomBase 10s ease-in-out infinite;
    transform-origin: center center;
}

.zoom-right {
    animation: zoomBase 4s ease-in-out infinite;
    transform-origin: 90% 80%; /* Your requested 3/4 to the right */
}

.zoom-left {
    animation: zoomBase 10s ease-in-out infinite;
    transform-origin: 20% center;
}

.zoom-bottom {
    animation: zoomBase 10s ease-in-out infinite;
    transform-origin: center 80%;
}

    
/* 3D Rotate + Fade */
.rotate-fade {
    animation: rotateFade 1.2s ease-out;
    perspective: 800px;
}

@keyframes rotateFade {
    0% { 
        transform: rotateY(15deg) scale(0.9); 
        opacity: 0; 
    }
    100% { 
        transform: rotateY(0) scale(1); 
        opacity: 1; 
    }
}

    
    
/* Add this to your existing <style> section */
.slide-left {
    animation-name: slideLeft;
    animation-duration: 1.5s;
}

@keyframes slideLeft {
    from {
        transform: translateX(100%);
        opacity: 0;
    }
    to {
        transform: translateX(0);
        opacity: 1;
    }
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

body {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        flex-direction: column;
        text-align: center;
        margin: 0;
    }

</style>

<h1 style="font-family: 'Playfair Display', serif; font-size: 5rem; font-weight: 700; color: #90ee90; text-align: center; transform: scaleX(2.5);">O G M A</h1>

Music and craic from the west of Ireland

<div class="slideshow-container">

    <!-- Slide 1 -->
    <div class="mySlides slide-left">
        <img src="/images/ogma1.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 2 -->
    <div class="mySlides zoom-right">
        <img src="/images/ogmaA3.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 3 -->
    <div class="mySlides rotate-fade">
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

<div class="video-grid">

  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/dQw4w9WgXcQ"
      title="Video 1"
      allowfullscreen>
    </iframe>
  </div>

  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/dQw4w9WgXcQ"
      title="Video 2"
      allowfullscreen>
    </iframe>
  </div>

  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/dQw4w9WgXcQ"
      title="Video 3"
      allowfullscreen>
    </iframe>
  </div>

  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/W_GasMIG1mM"
      title="Video 4"
      allowfullscreen>
    </iframe>
  </div>

  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/eDo8KBMemUk"
      title="Video 5"
      allowfullscreen>
    </iframe>
  </div>

  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/BSdAQUvnLNU"
      title="Video 6"
      allowfullscreen>
    </iframe>
  </div>

</div>

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
