<!-- Add icon library -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<h1 class="title">Team Members</h1>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Paige Riola" src="paige.jpg">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/paige-riola/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Paige Riola</h2>
    <p>I love AI and automation, so naturally I chose to help with UI on a
                                color picking app. I very much enjoy developing with friends, even
                                if it's outside of my comfort zone. My favorite color in the app is
                                called "Jedi Night" a deep dark green.</p>
  </div>
</div>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Gabriella Lindsey" src="gabby.jpg">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/gabriella-lindsey-8493951b0/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Gabriella Lindsey</h2>
    <p>I love AI and automation, so naturally I chose to help with UI on a
                                color picking app. I very much enjoy developing with friends, even
                                if it's outside of my comfort zone. My favorite color in the app is
                                called "Jedi Night" a deep dark green.</p>
  </div>
</div>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Dustin Seltz" src="dustin.jpg">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/dustin-s-7938a394/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Dustin Seltz</h2>
    <p>I love AI and automation, so naturally I chose to help with UI on a
                                color picking app. I very much enjoy developing with friends, even
                                if it's outside of my comfort zone. My favorite color in the app is
                                called "Jedi Night" a deep dark green.</p>
  </div>
</div>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Daniel Luft-Martinez" src="daniel.jpg">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/daniel-luft-martinez/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Daniel Luft-Martinez</h2>
    <span>I love AI and automation, so naturally I chose to help with UI on a
                                color picking app. I very much enjoy developing with friends, even
                                if it's outside of my comfort zone. My favorite color in the app is
                                called 
                                <div class="popup" onclick="onclickDaniel()">"Jedi Night"
                                  <span class="popupsquare" id="danielPopup">
                                    <div class="square" style="background-color: #041108;"></div>
                                    <b>HEX COLOR CODE<br>#041108</b>
                                  </span>
                                </div> a deep dark green.</span>
  </div>
</div>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Shealtiel Mulder" src="shealtiel.png">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/shealtiel-mulder-6329641b0/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Shealtiel Mulder</h2>
    <span>I enjoy creating beautiful UI experiences and using programming to
                                solve unique problems. I am very grateful for the opportunity to work
                                on this project alongside my colleagues and friends. My favourite color
                                in the app is called 
                                <div class="popup" onclick="onclickShealtiel()">"Aggressive Baby Blue"
                                  <span class="popupsquare" id="shealtielPopup"><div class="square" style="background-color: #6fffff;"></div></span>
                                </div> what a silly name!</span>
  </div>
</div>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Melanie Wong" src="melanie.jpg">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/mwong775/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Melanie Wong</h2>
    <span>I’m interested in learning and applying modern technologies such as 
                                mobile development and cloud computing to create meaningful experiences 
                                for users. My favorite color from the app is called 
                                <div class="popup" onclick="onclickMelanie()">"Blue Nebula"
                                  <span class="popupsquare" id="melaniePopup"><div class="square" style="background-color: #1199ff;"></div></span>
                                </div></span>
  </div>
</div>
<div class="row">
  <div class="profile">
    <div class="container">
      <img class="profileImg" alt="Andrew Tran" src="andrew.png">
      <div class="overlay">
        <a href="https://www.linkedin.com/in/andrewtgg/" class="icon" title="LinkedIn Profile">
          <i class="fa fa-linkedin"></i>
        </a>
      </div>
    </div>
  </div>
  <div class="message">
    <h2>Andrew Tran</h2>
    <p>I love AI and automation, so naturally I chose to help with UI on a
                                color picking app. I very much enjoy developing with friends, even
                                if it's outside of my comfort zone. My favorite color in the app is
                                called "Jedi Night" a deep dark green.</p>
  </div>
</div>

<script>
// When the user clicks on div, open the popup
function onclickDaniel() {
  var popup = document.getElementById("danielPopup");
  popup.classList.toggle("show");
}
  
function onclickShealtiel() {
  var popup = document.getElementById("shealtielPopup");
  popup.classList.toggle("show");
}

function onclickMelanie() {
  var popup = document.getElementById("melaniePopup");
  popup.classList.toggle("show");
}
</script>
