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
    background-color: rgba(0, 0, 0, 0.75); 
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






This is part of the technology and innovation seminar course at Webb.

Earlier this month, the Webb admission department approached us with a rather unique request: design DIY name plates for everyone in admissions. This will help them demonstrate Webb's mission, as well as giving an example to what students could expect in their time here. This project had several different parts, with the goal to produce several standardized name plates, several customized name plates, and two name plates for the school.

First, we did some divergent thinking, in which everyone proposed different visions as to how the name plates could look like. I contributed my own sketches with a 3D Webb lettering. 

I also helped some of my classmates figure out how to import DXF files into Onshape, the CAD program we were using. The Webb Schools logo is a standardized "font". Therefore, we could use tools such as Inkscape or Adobe Illustrator to convert the .svg file to a DXF file. Since Onshape is extremely sensitive to DXF sizing, it took several tries to successfully scale the DXF file to work with the Onshape interface. Ultimately, our team elected a combination of .svg conversion and direct font input from Fusion 360 to solve this problem.

<img src="{{ '/media/images/logo_dxf_test.png' | relative_url }}" alt="Test DXF import">

Since our group was on a tight time constraint, I proposed the laser cutter as a useful solution to rapidly iterate standardized plates. Compared to customized plates, which should be 3D and show some character but takes multiple hours to produce, a laser cutter could batch produce all the required standardized name plates in about 30 minutes. We selected acrylic material as it can have multiple colors and is more durable than wood MDF. Using my past experience in robotics, I was able to come up with a design that would make the text show. Taking inspiration from our robotics team's number plate, we were able to cut the outside profile of the name plate as well as insets for each of the letters using blue acrylic. Then, we could cut the letters themselves using a contrasting color acrylic, yellow or white. If needed, letters can also protrude out of the plate by cutting 6mm instead of 3mm acrylic sheets. By putting tape on the backside of the plate and attaching all the letters on the front, into their corresponding slots, the letters are thus cleanly visible. These standardized name plates require a 3D printed mount, though, but it could drastically cut down the printing time, especially the time taken for the nozzle to change out filament. The 3D printed mount was produced by another classmate whose initial design was adapted for this use as it was simple and suitable for the laser-cut flat plates. 

<img src="{{ '/media/images/IMG_0407.jpg' | relative_url }}" alt="A prototype">

I also helped create a short tutorial on how to use the laser cutter in this process. Here is a snapshot from the tutorial, addressing common power settings for different materials. I will expand upon this tutorial in the future to include a more comprehensive guide available.

<img src="{{ '/media/images/IMG_0697.jpg' | relative_url }}" alt="Tutorial">

</div>
