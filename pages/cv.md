---
layout: page
title: "CV"
meta_title: "CV | Dorien Huijser"
permalink: "/cv/"
sidebar: right
header: no
---

<html>
<head>
<style>
/* Style collapsible */
.collapsible {
  background-color: $ci-1;
  color: white;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
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
}

.collapsible:after {
content: '\002B'; /_ Unicode character for "plus" sign (+) _/
font-size: 20px;
color: black;
float: right;
margin-left: 5px;
}

.collapsible:active:after {
content: "\2212"; /_ Unicode character for "minus" sign (-) _/
}
</style>

</head>
</html>

Click a header to expand.

{% include cv.html %}
