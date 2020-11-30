---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Bio"
  url: '/bio/'
  image: widget-1-302x182.jpg
  text: 'Read more about my journey so far in my bio.'
widget2:
  title: "What I do"
  url: '/what-i-do/'
  text: 'Read more about what I do.'
  image: widget-1-302x182.jpg
widget3:
  title: "Testimonials"
  url: '/testimonials/'
  image: widget-github-303x182.jpg
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
        <meta name="viewport" content="width-device-width, initial-scale=1"></meta>
        <style>
            img{border-radius: 80%;}

​            

            figure {
      border: 0px #cccccc solid;
      padding: 0px;
      margin: auto;
    }
    
    figcaption {
      background-color: white;
      color: black;
      font-style: italic;
      padding: 2px;
      text-align: center;
    }
        </style>
            </head>


<body>



<p style="text-align:center;"><img src="images/nov2020_squarebw.jpg" alt="Profile picture" style="width:200px"></p>



<h1>
    <p style="text-align:center;">Welcome!</p>
</h1>
<p style="text-align:center;">You have somehow landed on my personal website, congratulations!<br>
Click on the menu above if you want to know more about me.
</p>

<h2>About me</h2>

<p>My name is Dorien. I am currently a research assistant, but I aspire to be much more than that title suggests. My current job mostly consists of building bridges:</p>

<div class="row">
  <div class="column" style="background-color:#FFFFFF;">
         <p><ul>
      <li>As data manager, I am the bridge between developmental psychologists (at the <a href="http://erasmus-synclab.nl/">SYNC lab</a> and the <a href="https://www.universiteitleiden.nl/onderzoek/onderzoeksprojecten/sociale-wetenschappen/leiden-consortium-on-individual-development-l-cid">L-CID study</a>) and their aims to work more in line with principles of open science. I do this by helping them get more information, looking for new research tools, connecting with other researchers and support staff about struggles we run into and educating myself with knowledge of others.</li>
    <li>As lab manager, I am the bridge between researchers and university-wide support staff to get practical things done. Moreover, because I also help with our citizen science initiatives, I am also part of the important two-way bridge we are building between our science and society.</li>
      </ul></p>
  </div>
  <div class="column" style="background-color:#FFFFFF;text-align:center">
      <figure>
 <img src="images/bridge.jpg" alt="Bridge building" style="zoom:50%;"/>
 <figcaption>
 <i>Source: <a href="https://pixabay.com/nl/photos/mist-bos-catwalk-brug-1957493/">Pixabay</a></i>
 </figcaption>
</figure>
    </div> </div>




<a class="twitter-timeline" data-lang="en" data-width="250" data-height="350" data-theme="light" href="https://twitter.com/DorienHuijser?ref_src=twsrc%5Etfw">Tweets by DorienHuijser</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>







