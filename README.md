
<h2 style="margin: auto;">About</h2>
---
Looking for a convenient color-picking experience on the go? Look no further than LiveColor. All it takes to get started is simply uploading a photo from your mobile device’s camera roll. From there you’ll be able to save colors directly from your own photos! Save your favorite colors, design your own palettes, generate complex harmonies, and even edit colors all within LiveColor.  

<h2 style="margin: auto;">Features</h2>
---

### Color Picking
<div class="flex-container">
  <img id="img1CP" class="step1CP" height="322" src="1-colorpicking.png">
  <img id="img2CP" class="step2CP" height="322" src="2-colorpicking.png">
  <img id="img3CP" class="step3CP" height="322" src="3-colorpicking.png">
  <p id="instruction1CP" class="instruction1CP">Begin by clicking the Add Image button. Then either take a photo with your device or upload a photo from your photo gallery.</p>
  <p id="instruction2CP" class="instruction2CP">After selecting the desired color by tapping the image, press the Save Color button to save the color.</p>
  <p id="instruction3CP" class="instruction3CP">Then click the Saved Colors icon on the bottom bar in order to see all the colors you have saved.</p>
</div>
<div class="center">
  <div class="pagination">
    <a id="link1CP" onclick="onStep1CP()" class="activeCP">1</a>
    <a id="link2CP" onclick="onStep2CP()">2</a>
    <a id="link3CP" onclick="onStep3CP()">3</a>
  </div>
</div>
---

### Color Info
<div class="flex-container">
  <img id="img1CI" class="step1CI" height="322" src="1-colorinfo.png">
  <img id="img2CI" class="step2CI" height="322" src="3-colorpicking.png"> <!--uses the same image so I'm resuing it to save space-->
  <img id="img3CI" class="step3CI" height="322" src="3-colorinfo.png"> 
  <p id="instruction1CI" class="instruction1CI">To view the color info for the currently selected color, click on the Info icon in the color description. To see color info for       colors you have already saved, go to your Saved Colors.</p>
  <p id="instruction2CI" class="instruction2CI">Once in your Saved Colors simply tap on a color to view its Color Info.</p>
  <p id="instruction3CI" class="instruction3CI">From here you can view and edit your colors in Hex, RGB, and HSV.</p>
</div>
<div class="center">
  <div class="pagination">
    <a id="link1CI" onclick="onStep1CI()" class="activeCI">1</a>
    <a id="link2CI" onclick="onStep2CI()">2</a>
    <a id="link3CI" onclick="onStep3CI()">3</a>
  </div>
</div>
---

### Generating Harmonies
<div class="flex-container">
  <img id="img1CH" class="step1CH" height="322" src="1-colorharmonies.png">
  <img id="img2CH" class="step2CH" height="322" src="colorharmonies.gif">
  <p id="instruction1CH" class="instruction1CH">Navigate to the Color Info of your desired color. Once there tap the <br>"VIEW COLOR HARMONIES" button on the bottom.</p>
  <p id="instruction2CH" class="instruction2CH">Scroll through our many automatically generated harmonies. If you find one you like, simply tap on it to display all the colors       in the harmony.</p>
</div>
<div class="center">
  <div class="pagination">
  <a id="link1CH" onclick="onStep1CH()" class="activeCH">1</a>
  <a id="link2CH" onclick="onStep2CH()">2</a>
  </div>
</div>
---

### Installation

- Download **[Android Studio](https://developer.android.com/studio)**
- Set up GitHub through Android Studio’s VCS options
- Download the project
- Using Android Studio’s AVD manager, set up and run an emulator using Pixel 2 API 27

## About Us
<a href="./credits.html">Meet the Team!</a>

<script>
 //these 3 functions switch between the 3 tutorial images for Color Picking (C.P.)
  function onStep1CP() {
    var x = document.getElementsByClassName("activeCP");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCP");
    }
    document.getElementById("link1CP").classList.add("activeCP");
    //
    document.getElementById("img1CP").style.display = "block";
    document.getElementById("img2CP").style.display = "none";
    document.getElementById("img3CP").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CP").style.display = "block";
    document.getElementById("instruction2CP").style.display = "none";
    document.getElementById("instruction3CP").style.display = "none";
  }
  
  function onStep2CP() {
    var x = document.getElementsByClassName("activeCP");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCP");
    }
    document.getElementById("link2CP").classList.add("activeCP");
    //
    document.getElementById("img1CP").style.display = "none";
    document.getElementById("img2CP").style.display = "block";
    document.getElementById("img3CP").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CP").style.display = "none";
    document.getElementById("instruction2CP").style.display = "block";
    document.getElementById("instruction3CP").style.display = "none";
  }
  
  function onStep3CP() {
    var x = document.getElementsByClassName("activeCP");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCP");
    }
    document.getElementById("link3CP").classList.add("activeCP");
    //
    document.getElementById("img1CP").style.display = "none";
    document.getElementById("img2CP").style.display = "none";
    document.getElementById("img3CP").style.display = "block";
    //Displays the correct instruction message
    document.getElementById("instruction1CP").style.display = "none";
    document.getElementById("instruction2CP").style.display = "none";
    document.getElementById("instruction3CP").style.display = "block";
  }
  
  //these 3 functions switch between the 3 tutorial images for Color Info (C.I.)
  function onStep1CI() {
    var x = document.getElementsByClassName("activeCI");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCI");
    }
    document.getElementById("link1CI").classList.add("activeCI");
    //
    document.getElementById("img1CI").style.display = "block";
    document.getElementById("img2CI").style.display = "none";
    document.getElementById("img3CI").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "block";
    document.getElementById("instruction2CI").style.display = "none";
    document.getElementById("instruction3CI").style.display = "none";
  }
  
  function onStep2CI() {
    var x = document.getElementsByClassName("activeCI");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCI");
    }
    document.getElementById("link2CI").classList.add("activeCI");
    //
    document.getElementById("img1CI").style.display = "none";
    document.getElementById("img2CI").style.display = "block";
    document.getElementById("img3CI").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "none";
    document.getElementById("instruction2CI").style.display = "block";
    document.getElementById("instruction3CI").style.display = "none";
  }
  
  function onStep3CI() {
    var x = document.getElementsByClassName("activeCI");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCI");
    }
    document.getElementById("link3CI").classList.add("activeCI");
    //
    document.getElementById("img1CI").style.display = "none";
    document.getElementById("img2CI").style.display = "none";
    document.getElementById("img3CI").style.display = "block";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "none";
    document.getElementById("instruction2CI").style.display = "none";
    document.getElementById("instruction3CI").style.display = "block";
  }
  
  //these 3 functions switch between the 3 tutorial images for Color Harmonies (C.H.)
  function onStep1CH() {
    var x = document.getElementsByClassName("activeCH");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCH");
    }
    document.getElementById("link1CH").classList.add("activeCH");
    //
    document.getElementById("img1CH").style.display = "block";
    document.getElementById("img2CH").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CH").style.display = "block";
    document.getElementById("instruction2CH").style.display = "none";
  }
  
  function onStep2CH() {
    var x = document.getElementsByClassName("activeCH");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCH");
    }
    document.getElementById("link2CH").classList.add("activeCH");
    //
    document.getElementById("img1CH").style.display = "none";
    document.getElementById("img2CH").style.display = "block";
    //Displays the correct instruction message
    document.getElementById("instruction1CH").style.display = "none";
    document.getElementById("instruction2CH").style.display = "block";
  }
</script>
