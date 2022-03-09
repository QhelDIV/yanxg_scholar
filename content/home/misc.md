---
# An instance of the Blank widget with a Gallery page element.
# Documentation: https://wowchemy.com/docs/getting-started/page-builder/
widget: blank

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 30

title: Misc
subtitle:

design:
  columns: '2'
#<!-- {{< gallery album="themes" >}} -->
---

<head>

<style>
  .hovereffect {
    width: 100%;
    height: 100%;
    float: left;
    overflow: hidden;
    position: relative;
    text-align: center;
    cursor: default;
  }
  .hovereffect .overlay {
    position: absolute;
    overflow: hidden;
    width: 80%;
    height: 80%;
    left: 10%;
    top: 10%;
    border-bottom: 1px solid #FFF;
    border-top: 1px solid #FFF;
    -webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
    transition: opacity 0.35s, transform 0.35s;
    -webkit-transform: scale(0,1);
    -ms-transform: scale(0,1);
    transform: scale(0,1);
  }
  .hovereffect:hover .overlay {
    opacity: 1;
    filter: alpha(opacity=100);
    -webkit-transform: scale(1);
    -ms-transform: scale(1);
    transform: scale(1);
  }
  .hovereffect img {
    display: block;
    position: relative;
    -webkit-transition: all 0.35s;
    transition: all 0.35s;
  }
  .hovereffect:hover img {
    filter: url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg"><filter id="filter"><feComponentTransfer color-interpolation-filters="sRGB"><feFuncR type="linear" slope="0.6" /><feFuncG type="linear" slope="0.6" /><feFuncB type="linear" slope="0.6" /></feComponentTransfer></filter></svg>#filter');
    filter: brightness(0.6);
    -webkit-filter: brightness(0.6);
  }
  .hovereffect h2 {
    text-transform: uppercase;
    text-align: center;
    position: relative;
    font-size: 17px;
    background-color: transparent;
    color: #FFF;
    padding: 1em 0;
    opacity: 0;
    filter: alpha(opacity=0);
    -webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
    transition: opacity 0.35s, transform 0.35s;
    -webkit-transform: translate3d(0,-100%,0);
    transform: translate3d(0,-100%,0);
  }
  .hovereffect a, .hovereffect p {
    color: #FFF;
    padding: 1em 0;
    opacity: 0;
    filter: alpha(opacity=0);
    -webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
    transition: opacity 0.35s, transform 0.35s;
    -webkit-transform: translate3d(0,100%,0);
    transform: translate3d(0,100%,0);
  }
  .hovereffect:hover a, .hovereffect:hover p, .hovereffect:hover h2 {
    opacity: 1;
    filter: alpha(opacity=100);
    -webkit-transform: translate3d(0,0,0);
    transform: translate3d(0,0,0);
  }

  .row {
    display: flex;
    flex-wrap: wrap;
    padding: 0 4px;
  }
  /* Create four equal columns that sits next to each other */
  .column {
    flex: 50%;
    max-width: 50%;
    padding: 0 4px;
  }
  .column img {
    margin-top: 8px;
    margin-bottom: 8px;
    vertical-align: middle;
    width: 100%;
    box-shadow: 3px 3px 3px #ccc;
  }
  /* Responsive layout - makes a two column-layout instead of four columns */
  @media screen and (max-width: 800px) {
    .column {
      flex: 50%;
      max-width: 50%;
    }
  }
  /* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
  @media screen and (max-width: 600px) {
    .column {
      flex: 100%;
      max-width: 100%;
    }
  }
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}
.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;

  /* Position the tooltip */
  position: absolute;
  z-index: 1;
}
.tooltip:hover .tooltiptext {
  visibility: visible;
}

</style>
<!-- <style>
  div.gallery {
    margin: 5px;
    border: 1px solid #ccc;
    float: left;
    width: 100%;
  }
  div.gallery:hover {
    border: 1px solid #777;
  }
  div.gallery img {
    width: 100%;
    height: 100%;
  }
  div.desc {
    padding: 1px;
    text-align: center;
  }
</style> -->
</head>
<body>

<p>
I am an endurance sports lover and have finished 1 full-Marathon, 7 half-Marathon and 1 triathlon.
I usually run 5 kilometers everyday and by the time of <b id="now_date"></b> my total mileage is <b id="mileage"></b> kilometers
</p>

<p>
I also like 3D modeling and rendering, the following shows several works of mine (some of them are interactive thanks to WebGL).
</p>

  <div class="row">
    <div class="column">
      <!-- <div class="tooltip"> -->
        <a href="media/images/hp_misc/yanxg_logo.png"><img src="media/images/hp_misc/yanxg_logo.png"></a> 
        <!-- <span class="tooltiptext">Tooltip text</span> 
      </div> -->
      <a href="media/images/hp_misc/hw1.jpg"><img src="media/images/hp_misc/hw1.jpg"></a>
      <a href="media/images/hp_misc/hw2.jpg"><img src="media/images/hp_misc/hw2.jpg"></a>
      <a href="GeometryGallery/arts/Stereographic_Projection.html"><img src="media/images/hp_misc/steographic.jpg"></a>
      <a href="NBodySimulation/"><img src="media/images/hp_misc/NBody.jpg"></a>
    </div>
    <div class="column">
      <a href="media/images/hp_misc/sunset.png"><img src="media/images/hp_misc/sunset.png"></a>
      <a href="media/images/hp_misc/hw53-01-01.jpg"><img src="media/images/hp_misc/hw53-01-01.jpg"></a>
      <a href="media/images/hp_misc/hw3.jpg"><img src="media/images/hp_misc/hw3.jpg"></a>
      <a href="GeometryGallery/arts/3D_Sierpinski_Triangle.html"><img src="media/images/hp_misc/triangle.jpg"></a>
      <a href="https://github.com/QhelDIV/MusicSynthesizer"><img src="media/images/hp_misc/musicgen.jpg"></a>
    </div>
  </div>
<br>

<script>
// Set the date we're counting down to
var startDate = new Date("Jan 15, 2022 23:59:59").getTime();
// Update the count down every 1 second
var x = setInterval(function() {
  // Get today's date and time
  var ndate = new Date()
  var now = ndate.getTime();
  // Find the distance between now and the count down date
  var distance = now - startDate;
    
  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
    
  // Output the result in an element with id="demo"
  // document.getElementById("demo").innerHTML = days + "d " + hours + "h "
  // + minutes + "m " + seconds + "s ";
  ny = ndate.getFullYear();
  nm = ndate.getMonth() + 1;
  nd = ndate.getDate();
  document.getElementById("now_date").innerHTML = ny + "."  + nm + "." + nd;
  document.getElementById("mileage").innerHTML  = 2939.3 + 5.0*days 
  // If the count down is over, write some text 
  // if (distance < 0) {
  //   clearInterval(x);
  //   document.getElementById("demo").innerHTML = "EXPIRED";
  // }
}, 1000);
</script>

<!-- <div class="gallery">
  <a target="_blank" href="media/images/tn.png">
    <img src="media/images/tn.png" alt="Mountains" width="100%" height="100%">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>
<div class="gallery">
  <a target="_blank" href="media/images/tn.png">
    <img src="media/images/tn.png" alt="Mountains" width="100%" height="100%">
  </a>
  <div class="desc">Add a description of the image here</div>
</div> -->


</body>