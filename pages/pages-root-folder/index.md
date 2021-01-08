---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  title: "Dorien Huijser"
  image_fullwidth: home.jpg
widget1:
  title: "Bio"
  url: '/bio/'
  image: nov2020_squarebw2.jpg
  text: 'Read more about my journey so far.'
widget2:
  title: "What I do"
  url: '/what-i-do/'
  text: 'Read more about what I do.'
  image: bridgesq.jpg
widget3:
  title: "Testimonials"
  url: '/testimonials/'
  image: talkingsq.jpg
  text: 'Who better to say stuff about me than... <em>not me</em>? Read what others say about me on this page'
# Use the call for action to show a button on the frontpage
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: /contact/
  text: Get in touch! ›
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
</style>

<body>



<figure style="border:0px #cccccc solid; padding:0px; margin:auto;text-align:center"><img src="images/nov2020_squarebw.jpg" alt="Profile picture" style="width:200px;border-radius:80%;"></figure>



<h1><p style="text-align:center;">Welcome!</p></h1>
<p style="text-align:center;">You have landed on my personal website, congratulations! <br> On this website, you can read more about me and what I do. </p><br>

<div class="row">
  <div class="column" style="background-color:#FFFFFF;">
         <ul>
      <li>As <strong>data manager</strong>, I am the bridge between developmental psychologists (at the <a href="http://erasmus-synclab.nl/">SYNC lab</a> and the <a href="https://www.universiteitleiden.nl/onderzoek/onderzoeksprojecten/sociale-wetenschappen/leiden-consortium-on-individual-development-l-cid">L-CID study</a>) and their aims to work more in line with principles of <strong>open science</strong>. I help them get more information, look for new research tools and connect with other researchers and support staff about struggles we run into.</li></ul></div>
<div class="column" style="background-color:#FFFFFF;">
    <ul>
      <li>As <strong>lab manager</strong>, I am the bridge between researchers and university-wide support staff to get practical things done. Moreover, I help with our <strong>citizen science</strong> initiative "YoungXperts", building a two-way bridge between our science and society.</li>  
    </ul>
    </div>

<h2>
    Bio
</h2>

<div class="container">
  <img src="../../images/las2.jpg" style="zoom:60%;" >
  <div class="bottom-left"><h3>Studies</h3></div>
</div>
<p>I started my career at Utrecht University in the bachelor <a href="https://www.uu.nl/bachelors/liberal-arts-and-sciences">Liberal Arts and Sciences</a>. Here, I learned about the importance of <b>interdisciplinary cooperation</b> as a way to solve society's larger issues. Additionally, I dove into <b>Cognitive and neurobiological psychology</b> (major) and <b>Language development</b> (minor).</p>

<p>In my master <a href="https://www.uu.nl/masters/en/neuroscience-and-cognition">Neuroscience and Cognition</a>, I conducted two <b>research projects</b> in both cognitive (9 months) and developmental psychology (6 months). Additionally, I completed a minor in <b>science education and communication</b>, where I gained skills in communicating science to different audiences.</p>

<div class="container">
  <img src="../../images/work.jpg" style="zoom:60%">
  <div class="bottom-left"><h3>Work</h3></div>
</div>
<p>After my master's, I started as <b>data manager</b> at the Brain and Development Research Center ánd as <b>educational content creator and e-moderator</b> at University Medical Center Utrecht (UMC). In these positions, I was able to combine promoting good research practices with creating educational scientific content for a PhD audience.</p>

<p>Currently, I work as a research assistant at Erasmus University Rotterdam (<a href="https://www.eur.nl/people/dorien-huijser">EUR</a>) and Leiden University <a href="https://www.universiteitleiden.nl/en/staffmembers/dorien-huijser">LU</a>), fullfilling the tasks of <b>data and lab manager</b> (see above).</p>

