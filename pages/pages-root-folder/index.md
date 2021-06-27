---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
meta_title: "Home | Dorien Huijser"
header:
  title: "Dorien Huijser"
  image_fullwidth: home.jpg
widget1:
  title: "What I do"
  url: "/what-i-do/"
  image: bridgesq.jpg
  text: "Read more about what I do."
widget2:
  title: "Testimonials"
  url: "/testimonials/"
  text: "Who better to say stuff about me than... <em>not me</em>? Read what others say about me on this page."
  image: talkingsq.jpg
widget3:
  title: "CV"
  url: "/cv/"
  image: nov2020_squarebw2.jpg
  text: "Checkout all my qualifications and work experience here."
# Use the call for action to show a button on the frontpage
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: /contact/
  text: Get in touch
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<html>

    <head>
        <meta name="viewport" content="width-device-width, initial-scale=1">
        </head>

<style>
    /* Columns on a page */
    .container {
  position: relative;
  text-align: left;
}
.bottom-left {
  position: absolute;
  bottom: 8px;
  left: 16px;
}
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.column {
 float: left;
 width: 50%;
}

/* Clear floats after the columns */
.row:after {
 content: "";
 display: table;
 clear: both;
}

/* Code to create collapsible */

.collapsible {
  background-color: $ci-1;
  color: white;
  cursor: pointer;
  padding: 10px;
  width: 30%;
  border: none;
  text-align: center;
  outline: none;
  font-size: large;
}

.active, .collapsible:hover {
  background-color: $ci-2;
}

.content {
  padding: 0 18px;
  display: none;
  overflow: hidden;
  background-color: #fff;
  text-align: left;
}

.collapsible:after {
  content: '\002B'; /* Unicode character for "plus" sign (+) */
  font-size: 20px;
  color: black;
  float: right;
  margin-left: 5px;
}

.collapsible:active:after {
  content: "\2212"; /* Unicode character for "minus" sign (-) */
}

</style>

<body>

<br>

<div><figure style="border:0px #cccccc solid; padding:0px; margin:auto;text-align:center"><img src="../../images/nov2020_squarebw.jpg" alt="Profile picture" style="width:200px;border-radius:80%;"></figure></div>

<br>

<h1 style="text-align:center"><p style="text-align:center;">Welcome!</p></h1>
<p style="text-align:center;">You have landed on my personal website! <br> Here, you can read more about me and what I do. </p>

<br>

<div style="text-align:center"><button type="button" class="collapsible"><b>Bio</b></button>

<div class="content">
<div class="row">
    <div class="column">
<p><div class="container">
  <img src="../../images/las2.jpg" style="zoom:100%;" >
  <div class="bottom-left"><h3 style="color:white">Studies</h3></div>
</div>
<p  style="text-align:left">I started my career at Utrecht University in the bachelor <a href="https://www.uu.nl/bachelors/liberal-arts-and-sciences">Liberal Arts and Sciences</a>. Here, I learned about the importance of <b>interdisciplinary cooperation</b> as a way to solve society's larger issues. Additionally, I dove into <b>Cognitive and neurobiological psychology</b> (major) and <b>Language development</b> (minor).</p></p>
    <p>In my master <a href="https://www.uu.nl/masters/en/neuroscience-and-cognition">Neuroscience and Cognition</a>, I conducted two <b>research projects</b> in both cognitive (9 months) and developmental psychology (6 months). Additionally, I completed a minor in <b>science education and communication</b>, where I gained skills in communicating science to different audiences.</p></div>
    <div class="column"><p><div class="container">
  <img src="../../images/work.jpg" style="zoom:100%">
  <div class="bottom-left"><h3 style="color:white">Work</h3></div>
</div>
<p>After my master's, I started as educational content creator and e-moderator at UMC Utrecht, and as a data manager at the Brain and Development Research Center. In these positions, I was able to combine promoting good research practices with creating educational scientific content for a PhD audience. Later, I continued my job as a data manager at the same developmental neuroscience group at Erasmus University Rotterdam and Leiden University.</p></p>
<p>Currently, I work as a data steward at the Utrecht University Library. In this position, I help researchers with their research data management questions and issues. Check out the <a href="../what-i-do">What I do page</a> for more info.</p></div></div>
</div></div>

<script>
/* script for creating a collapsible element */
    var coll = document.getElementsByClassName("collapsible");
var i;
for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
    } else {
      content.style.display = "block";
    }
  });
}
</script>

</body>

</html>
