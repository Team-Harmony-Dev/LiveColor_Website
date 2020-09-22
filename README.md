
<h2 style="margin: auto;">About</h2>

Looking for a convenient color-picking experience on the go? Look no further than LiveColor. All it takes to get started is simply uploading a photo from your mobile device’s camera roll. From there you’ll be able to save colors directly from your own photos! Save your favorite colors, design your own palettes, generate complex harmonies, and even edit colors all within LiveColor.  

<h2 style="margin: auto;">Features</h2>


### Color Picking

<img id="img1" class="step1" height="322" src="color_picker.gif">
<img id="img2" class="step2" height="322" src="color_info.png">
<img id="img3" class="step3" height="322" src="harmonies.png">
<div class="center">
  <div class="pagination">
  <a onclick="onStep1()" class="active">1</a>
  <a onclick="onStep2()">2</a>
  <a onclick="onStep3()">3</a>
  </div>
</div>
---

### Color Info

<img height="322" src="color_info.png">

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
 //these 3 functions switch between the 3 tutorial images
  function onStep1() {
    var x = document.getElementsByClassName("active");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("active");
    }
    document.getElementById("img1").style.display = "block";
    document.getElementById("img1").classList.add("active");
    document.getElementById("img2").style.display = "none";
    document.getElementById("img3").style.display = "none";
  }
  
  function onStep2() {
    var x = document.getElementsByClassName("active");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("active");
    }
    document.getElementById("img1").style.display = "none";
    document.getElementById("img2").style.display = "block";
    document.getElementById("img2").classList.add("active");
    document.getElementById("img3").style.display = "none";
  }
  
  function onStep3() {
    var x = document.getElementsByClassName("active");
    var i;
    for (i = 0; i < x.length; i++) {
      x[i].classList.remove("active");
    }
    document.getElementById("img1").style.display = "none";
    document.getElementById("img2").style.display = "none";
    document.getElementById("img3").style.display = "block";
    document.getElementById("img3").classList.add("active");
  }
</script>
