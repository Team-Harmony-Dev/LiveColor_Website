
<h2 style="margin: auto;">About</h2>

Looking for a convenient color-picking experience on the go? Look no further than LiveColor. All it takes to get started is simply uploading a photo from your mobile device’s camera roll. From there you’ll be able to save colors directly from your own photos! Save your favorite colors, design your own palettes, generate complex harmonies, and even edit colors all within LiveColor.  

<h2 style="margin: auto;">Features</h2>


### Color Picking

<img id="img1CP" class="step1CP" height="322" src="color_picker.gif">
<img id="img2CP" class="step2CP" height="322" src="color_info.png">
<img id="img3CP" class="step3CP" height="322" src="harmonies.png">
<div class="center">
  <div class="pagination">
  <a id="link1CP" onclick="onStep1CP()" class="activeCP">1</a>
  <a id="link2CP" onclick="onStep2CP()">2</a>
  <a id="link3CP" onclick="onStep3CP()">3</a>
  </div>
</div>
---

### Color Info

---

### Harmonies

<img height="322" src="harmonies.png">

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
    document.getElementById("CPlink1").classList.add("activeCP");
    //
    document.getElementById("img1CP").style.display = "block";
    document.getElementById("img2CP").style.display = "none";
    document.getElementById("img3CP").style.display = "none";
  }
  
  function CPonStep2() {
    var x = document.getElementsByClassName("CPactive");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("CPactive");
    }
    document.getElementById("CPlink2").classList.add("CPactive");
    //
    document.getElementById("CPimg1").style.display = "none";
    document.getElementById("CPimg2").style.display = "block";
    document.getElementById("CPimg3").style.display = "none";
  }
  
  function CPonStep3() {
    var x = document.getElementsByClassName("CPactive");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("CPactive");
    }
    document.getElementById("CPlink3").classList.add("CPactive");
    //
    document.getElementById("CPimg1").style.display = "none";
    document.getElementById("CPimg2").style.display = "none";
    document.getElementById("CPimg3").style.display = "block";
  }
</script>
