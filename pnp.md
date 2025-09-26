<style>
  body {
    margin: 0;
  }
  
  .video-background-holder {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -100;
    overflow: hidden;
  }
  
  #bg-video {
    width: 100vw;
    height: 100vh;
    object-fit: cover;
  }
  
  .overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5); 
    z-index: 1;
  }

  .content {
    color: white;
    position: relative; 
    z-index: 2; 
    padding: 2rem;
  }

  .content,
  .content * {
    color: white !important;
  }
</style>

<div class="video-background-holder">
  <video playsinline autoplay muted loop id="bg-video">
    <source src="/media/videos/IMG_0553.mp4" type="video/mp4">
  </video>
</div>

<div class="overlay"></div>

<div class="content" markdown="1">

# Project Name Plate

This is part of the technology and innovation seminar.

</div>
