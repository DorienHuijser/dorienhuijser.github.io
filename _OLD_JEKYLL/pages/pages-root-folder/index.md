---
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
layout: frontpage
meta_title: "Home | Dorien Huijser"
header:
  image_fullwidth: home.jpg
  title: ""
# Use the call for action to show a button on the frontpage
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
callforaction:
  url: /contact/
  text: Get in touch
  style: alert
permalink: /index.html
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
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
</style>

<body>

  <div class="row">
    <div class="column">
      <p>
          <div><figure style="border:0px #cccccc solid; padding:0px; margin:auto;text-align:center">
            <img src="../../images/nov2020_squarebw.jpg" alt="Profile picture" style="width:200px;border-radius:80%;"></figure>
          </div>
          <h1 style="text-align:center">Welcome!</h1>
          <p style = "text-align:center">
            You have landed on my personal website!
          </p>
          <p>
            Here, you can find out <a href="../what-i-do" target="_blank">what exactly I do</a> and  
          <a href="../cv" target = "_blank">what I have done in the past</a>. 
          If you have a question, feel free to contact me <a href="../contact" target = "_blank">via the form here</a> 
          or send me a message via <a href="https://www.uu.nl/staff/DCHuijser" target = "_blank">work email</a> or
          <a href="https://twitter.com/DorienHuijser" target = "_blank">Twitter</a>. 
          </p>
      </p>
    </div>
    <div class="column">
      <p>
        <h1>About</h1>
        <p>
          Hi! My name is Dorien. I am currently a research data manager at the Utrecht University Library, providing support for researchers
          surrounding the management of their data. In the past, I was the data manager in a developmental neuroscience group, where I focused
          on not only data management, but also other aspects of open science (e.g., data sharing, publishing open access, preregistrations, etc.)
          within the field of developmental neuroscience. I also have some educational experience in developing and moderating a online course 
          on designing animal experiments, and tutoring high schoolers. During my studies, I gained
          experience in, among others, working in an interdisciplinary way and performing research myself. These experiences have helped me
          navigate my current job. However, I'm always looking for more skills to learn during both my professional and personal journey!
        </p>
      </p>
    </div>
  </div>

</body>
</html>
