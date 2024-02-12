<!DOCTYPE html>
<html>
<head>
 <style>/* Style the buttons that are used to open and close the accordion panel */
.accordion {
  background-color: #eee;
  color: #444;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  text-align: left;
  border: none;
  outline: none;
  transition: 0.4s;
}

/* Add a background color to the button if it is clicked on (add the .active class with JS), and when you move the mouse over it (hover) */
.active, .accordion:hover {
  background-color: #ccc;
}

/* Style the accordion panel. Note: hidden by default */
.panel {
  padding: 0 18px;
  background-color: white;
  display: none;
  overflow: hidden;
}</style>
 <title>Kalon Ridley's Portfolio</title> 
</head>

<body>
 <div id="introduction"> <p><h1>Kalon Ridley's Portfolio</h1>
  For Dominican University</p></div>
  <div>
   <button class="accordion">Goal 1</button>
<div class="panel">
<p>Develop a professional identity and philosophy within the library and information professions.</p>
</div>
   <ul><li>Outcome 1a</li>
  <li>Outcome 1b</li>
  <li>Outcome 1c</li>
   </ul>
  </div>
  <div><h2>Goal 2</h2></div>
  <div><h2>Goal 3</h2></div>
  <div><h2>Goal 4</h2></div>
  <div><h2>Goal 5</h2></div>
</body>
<script>var acc = document.getElementsByClassName("accordion");
var i;

for (i = 0; i < acc.length; i++) {
  acc[i].addEventListener("click", function() {
    /* Toggle between adding and removing the "active" class,
    to highlight the button that controls the panel */
    this.classList.toggle("active");

    /* Toggle between hiding and showing the active panel */
    var panel = this.nextElementSibling;
    if (panel.style.display === "block") {
      panel.style.display = "none";
    } else {
      panel.style.display = "block";
    }
  });
}</script>
</html>
