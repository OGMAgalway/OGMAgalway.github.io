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

/* The animation keyframes */
@keyframes panInOut {
    0% {
        transform: translateX(100%); /* Start off-screen to the right */
        opacity: 0;
    }
    40% {
        transform: translateX(0); /* Pan in to the center */
        opacity: 1;
    }
    60% {
        transform: translateX(0); /* Stay in the center (pause) */
        opacity: 1;
    }
    100% {
        transform: translateX(-100%); /* Vanish off-screen to the left */
        opacity: 0;
    }
}

/* The class to apply to your slide */
.pan-in-out {
    animation-name: panInOut;
    animation-duration: 4s; /* Total duration for the whole sequence */
    animation-timing-function: ease-in-out;
    animation-fill-mode: forwards; /* Stops the slide at its final state */
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
    animation: zoomBase 4s cubic-bezier(0.68, -0.55, 0.27, 1.55) forwards;
    transform-origin: 90% 60%; /* Your requested 3/4 to the right */
}

.zoom-CR {
    animation: zoomBase 4s cubic-bezier(0.25, -0.8, 0.75, 1.8) forwards;
    transform-origin: 60% 1%;
}

.zoom-CRR {
    animation: zoomBase 4s cubic-bezier(0.25, -0.8, 0.75, 1.8) forwards;
    transform-origin: 95% 5%;
}
    
.zoom-CL {
    animation: zoomBase 4s cubic-bezier(0.68, -0.55, 0.27, 1.55) forwards;
    transform-origin: 25% 80%;
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

<h1 style="font-family: 'Caveat', serif; font-size: 7rem; font-weight: 700; color: #90ee90; text-align: center; transform: scaleX(2.5);">O G M A</h1>

<h1 style="font-family: 'Caveat', serif; font-size: 24px; font-weight: 700; color: white; text-align: center; transform: scaleX(2.5);">MUSIC AND CRAIC FROM THE WEST OF IRELAND</h1>


<div class="slideshow-container">

    <!-- Slide 2 -->
    <div class="mySlides zoom-right">
        <img src="/images/ogmaA3.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 1 -->
    <div class="mySlides pan-in-out">
        <img src="/images/ogma7b.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>
    
    <!-- Slide 3 -->
    <div class="mySlides zoom-CR">
        <img src="/images/ogmaC.jpg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 1 -->
    <div class="mySlides pan-in-out">
        <img src="/images/ogmaB3b.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>

    <!-- Slide 3 -->
    <div class="mySlides zoom-CL">
        <img src="/images/ogmaA2.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>
    
    <!-- Slide 1 -->
    <div class="mySlides pan-in-out">
        <img src="/images/ogmaE1.jpeg" alt="Band photo 1">
        <div class="text"></div>
    </div>
    
    <!-- Slide 3 -->
    <div class="mySlides zoom-CRR">
        <img src="/images/ogmaD1.jpg" alt="Band photo 1">
        <div class="text"></div>
    </div>

</div>


contact: [<a href="mailto:OPENTRAD@YAHOO.COM">OPENTRAD@YAHOO.COM</a>]

<style>
.three-columns {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}

.left-column {
    background-color: black;
    padding: 40px;
    text-align: left;
}

.mid-column {
    background-color: black;
    padding: 40px;
    text-align: left;
}

.right-column {
    background-color: black;
    padding: 40px;
    text-align: left;
}
</style>

<div class="three-columns">
    <div class="left-column">
        <span style="font-family:'Merienda', cursive; font-size:18px;">
                Occasionally playing with 
        fewer or more musicians, OGMA normally plays as a 4-piece. With occasional 
        substitutions, we are
        <ul>
            <li>
                <b>|Richard Hennessy|</b> <span style="font-family:'Ultra', serif; font-size:16px;"> vocals, guitar, banjo, bouzouki</span>
            </li>
            <li>
                <b>|Michael Mc Gettrick|</b><span style="font-family:'Ultra', serif; font-size:16px;"> tin whistle, clarinet, low whistle, concertina</span>
            </li>
            <li>
                <b>|Hugh Melvin|</b> <span style="font-family:'Ultra', serif; font-size:16px;"> flute, vocals, tin whistle, spoons</span>
            </li>
            <li>
                <b>|Cathal Seioghe|</b> <span style="font-family:'Ultra', serif; font-size:16px;"> fiddle, viola</span>
            </li>
        </ul>
        </span>
    </div>
    <div class="mid-column">
    <div class="video-grid">

<div class="video-container">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/orCbHD6lxL4"
      title="Video 1"
      allowfullscreen>
    </iframe>
  </div>
</div>

<div class="video-container">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/48uJyNcZ7Nc"
      title="Video 2"
      allowfullscreen>
    </iframe>
  </div>
</div>

<div class="video-container">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/rbjwUWioUpg"
      title="Video 3"
      allowfullscreen>
    </iframe>
  </div>
</div>

<div class="video-container">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/W_GasMIG1mM"
      title="Video 4"
      allowfullscreen>
    </iframe>
  </div>
</div>

<div class="video-container">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/vPL60l1Ybso"
      title="Video 5"
      allowfullscreen>
    </iframe>
  </div>
</div>

<div class="video-container">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/BSdAQUvnLNU"
      title="Video 6"
      allowfullscreen>
    </iframe>
  </div>
</div>

</div>
    </div>
    <div class="right-column">
        <span style="font-family:'Merienda', cursive; font-size:18px;">
        As well as playing weekly trad sessions in our home town (Galway City), we have performed
        <ul>
            <li>
                <b> many years in Switzerland (Lausanne, Fribourg, Berne, Bulle,...)</b> 
            </li>
            <li>
                <b> for two successive presidents of Ireland at &#193;ras an Uachtar&#225;in (current President Connolly, previous
                President Higgins)</b> 
            </li>
            <li>
                <b> for large events at Guinness Storehouse, Dublin </b> 
            </li>
            <li>
                <b> at Cork Folk Festival</b> 
            </li>
            <li>
                <b> at many different conferences, festivals and events in Galway City</b> 
            </li>
        </ul>
        </span>
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
