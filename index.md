---
title: "Wind & Temperature Measurement"
author: "Lala NG"
highlighter: highlight.js
output: pdf_document
job: null
knit: slidify::knit2slides
mode: selfcontained
hitheme: tomorrow
subtitle: Data Product Development
framework: io2012
widgets: []
---

## Objectives

1. Demonstrate the ability of using basic shiny app
2. Slide 1: reactive output display with isolate. GGplot2 is used. Temperature on Monthly basis is recorded.
3. Slide 2: rCharts integration for Wind Measurement on regular daily basis
4. Data Source Interaction - airquality.

Warning: For some reasons, the app occasionally fails to get resource from shiny server. Please evaluate my apps locally.

--- .class #id 

## Temperature Measurement on Monthly basis

{{{ content }}}
<footer class = 'logo'>
  <img src = 'slide1.png' height="500px"></img>
</footer>


This is the link to the shiny app: https://lalang.shinyapps.io/dataproduct/


---
## Wind Measurement classified by Day
<iframe src=' assets/fig/unnamed-chunk-1-1.html ' scrolling='no' frameBorder='0' seamless class='rChart polycharts ' id=iframe- chart1 ></iframe> <style>iframe.rChart{ width: 100%; height: 400px;}</style>

This is the link to the shiny app: https://lalang.shinyapps.io/dataproduct/

---
## Data Source Interaction 
{{{ content }}}
<footer class = 'logo'>
  <img src = 'slide3.png' height="500px"></img>
</footer>


This is the link to the shiny app: https://lalang.shinyapps.io/dataproduct/
