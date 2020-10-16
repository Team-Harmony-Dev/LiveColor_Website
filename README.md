
<a href='https://play.google.com/store/apps/details?id=com.harmony.livecolor&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png'/></a>



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

### Color Info & Editing
<div class="flex-container">
  <img id="img1CI" class="step1CI" height="322" src="1-colorinfo.png">
  <img id="img2CI" class="step2CI" height="322" src="3-colorpicking.png"> <!--uses the same image so I'm resuing it to save space-->
  <img id="img3CI" class="step3CI" height="322" src="3-colorinfo.png"> 
  <img id="img4CI" class="step4CI" height="322" src="4-colorinfo.png"> 
  <p id="instruction1CI" class="instruction1CI">To view the color info for the currently selected color, click on the Info icon in the color description. To see color info for       colors you have already saved, go to your Saved Colors.</p>
  <p id="instruction2CI" class="instruction2CI">Once in your Saved Colors simply tap on a color to view its Color Info.</p>
  <p id="instruction3CI" class="instruction3CI">From here you can view and edit your colors in HEX, RGB, and HSV. To edit a color, tap the pencil icon in the top right.</p>
  <p id="instruction4CI" class="instruction4CI">Modify your color in RGB or HSV with live comparison to the original color.</p>
</div>
<div class="center">
  <div class="pagination">
    <a id="link1CI" onclick="onStep1CI()" class="activeCI">1</a>
    <a id="link2CI" onclick="onStep2CI()">2</a>
    <a id="link3CI" onclick="onStep3CI()">3</a>
    <a id="link4CI" onclick="onStep4CI()">4</a>
  </div>
</div>
---

### Generating Harmonies
<div class="flex-container">
  <img id="img1CH" class="step1CH" height="322" src="1-colorharmonies.png">
  <img id="img2CH" class="step2CH" height="322" src="colorharmonies.gif">
  <img id="img3CH" class="step3CH" height="322" src="3-colorharmonies.png">
  <p id="instruction1CH" class="instruction1CH">Navigate to the Color Info of your desired color. Once there tap the <br>"VIEW COLOR HARMONIES" button on the bottom.</p>
  <p id="instruction2CH" class="instruction2CH">Scroll through our many automatically generated harmonies. If you find one you like, simply tap on it to display all the colors       in the harmony.</p>
  <p id="instruction3CH" class="instruction3CH">From here, you can look at the info for any of the colors in the palette as you would for any other color! If you like the           palette and want to save it, you can hit the save button in the top right corner and set a name for your new palette.</p>
</div>
<div class="center">
  <div class="pagination">
    <a id="link1CH" onclick="onStep1CH()" class="activeCH">1</a>
    <a id="link2CH" onclick="onStep2CH()">2</a>
    <a id="link3CH" onclick="onStep3CH()">3</a>
  </div>
</div>
---

### Color of the Day
<img class="step1COTD" height="322" src="cotd.png">
<p class="instruction1COTD">Discover and appreciate a different color every day with our Color of The Day feature! You might even get a special color for certain holidays!</p>
---

### Customization & Settings
<div class="flex-container">
  <img id="img1CS" class="step1CS" height="322" src="1-settings.png">
  <img id="img2CS" class="step2CS" height="322" src="2-settings.png">
  <img id="img3CS" class="step3CS" height="322" src="darkmode.png">
  <p id="instruction1CS" class="instruction1CS">To access Settings for the LiveColor app click the cog icon on the bottom right.</p>
  <p id="instruction2CS" class="instruction2CS">Tweak any of our app settings to match your preferences. Check out the "Appearance" settings page to try out Dark Mode.</p>
  <p id="instruction3CS" class="instruction3CS">From here Enable or Disable Dark Mode for the app. Type or paste in a hex value for the accent color for the current mode: Dark        or Light.</p>
</div>
<div class="center">
  <div class="pagination">
  <a id="link1CS" onclick="onStep1CS()" class="activeCS">1</a>
  <a id="link2CS" onclick="onStep2CS()">2</a>
  <a id="link3CS" onclick="onStep3CS()">3</a>
  </div>
</div>
---

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
  
  //these 4 functions switch between the 4 tutorial images for Color Info (C.I.)
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
    document.getElementById("img4CI").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "block";
    document.getElementById("instruction2CI").style.display = "none";
    document.getElementById("instruction3CI").style.display = "none";
    document.getElementById("instruction4CI").style.display = "none";
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
    document.getElementById("img4CI").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "none";
    document.getElementById("instruction2CI").style.display = "block";
    document.getElementById("instruction3CI").style.display = "none";
    document.getElementById("instruction4CI").style.display = "none";
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
    document.getElementById("img4CI").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "none";
    document.getElementById("instruction2CI").style.display = "none";
    document.getElementById("instruction3CI").style.display = "block";
    document.getElementById("instruction4CI").style.display = "none";
  }
  
  function onStep4CI() {
    var x = document.getElementsByClassName("activeCI");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCI");
    }
    document.getElementById("link4CI").classList.add("activeCI");
    //
    document.getElementById("img1CI").style.display = "none";
    document.getElementById("img2CI").style.display = "none";
    document.getElementById("img3CI").style.display = "none";
    document.getElementById("img4CI").style.display = "block";
    //Displays the correct instruction message
    document.getElementById("instruction1CI").style.display = "none";
    document.getElementById("instruction2CI").style.display = "none";
    document.getElementById("instruction3CI").style.display = "none";
    document.getElementById("instruction4CI").style.display = "block";
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
    document.getElementById("img3CH").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CH").style.display = "block";
    document.getElementById("instruction2CH").style.display = "none";
    document.getElementById("instruction3CH").style.display = "none";
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
    document.getElementById("img3CH").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CH").style.display = "none";
    document.getElementById("instruction2CH").style.display = "block";
    document.getElementById("instruction3CH").style.display = "none";
  }
  
  function onStep3CH() {
    var x = document.getElementsByClassName("activeCH");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCH");
    }
    document.getElementById("link3CH").classList.add("activeCH");
    //
    document.getElementById("img1CH").style.display = "none";
    document.getElementById("img2CH").style.display = "none";
    document.getElementById("img3CH").style.display = "block";
    //Displays the correct instruction message
    document.getElementById("instruction1CH").style.display = "none";
    document.getElementById("instruction2CH").style.display = "none";
    document.getElementById("instruction3CH").style.display = "block";
  }
  
  //these 3 functions switch between the 3 tutorial images for Customization and Settings. (C.S.)
  function onStep1CS() {
    var x = document.getElementsByClassName("activeCS");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCS");
    }
    document.getElementById("link1CS").classList.add("activeCS");
    //
    document.getElementById("img1CS").style.display = "block";
    document.getElementById("img2CS").style.display = "none";
    document.getElementById("img3CS").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CS").style.display = "block";
    document.getElementById("instruction2CS").style.display = "none";
    document.getElementById("instruction3CS").style.display = "none";
  }
  
  function onStep2CS() {
    var x = document.getElementsByClassName("activeCS");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCS");
    }
    document.getElementById("link2CS").classList.add("activeCS");
    //
    document.getElementById("img1CS").style.display = "none";
    document.getElementById("img2CS").style.display = "block";
    document.getElementById("img3CS").style.display = "none";
    //Displays the correct instruction message
    document.getElementById("instruction1CS").style.display = "none";
    document.getElementById("instruction2CS").style.display = "block";
    document.getElementById("instruction3CS").style.display = "none";
  }
  
  function onStep3CS() {
    var x = document.getElementsByClassName("activeCS");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("activeCS");
    }
    document.getElementById("link3CS").classList.add("activeCS");
    //
    document.getElementById("img1CS").style.display = "none";
    document.getElementById("img2CS").style.display = "none";
    document.getElementById("img3CS").style.display = "block";
    //Displays the correct instruction message
    document.getElementById("instruction1CS").style.display = "none";
    document.getElementById("instruction2CS").style.display = "none";
    document.getElementById("instruction3CS").style.display = "block";
  }
</script>
