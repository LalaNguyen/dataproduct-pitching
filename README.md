---
title: "Wind & Temperature Measurement"
author: "Lala NG"
highlighter: highlight.js
mode: selfcontained
hitheme: tomorrow
knit        : slidify::knit2slides
subtitle: Data Product Development
framework: io2012
widgets: []
---

## Objectives

1. Demonstrate the ability of using basic shiny app
2. In Slide 1, reactive output display with isolate. GGplot2 is used. Temperature on Monthly basis is recorded.
3. In Slide 2, rCharts integration for Wind Measurement on regular daily basis
4. Data Source Interaction - airquality.

---

## Temperature Measurement on Monthly basis
Temperature is remarkbly higher in middle of summer.
<footer class = 'logo'>
  <img src = 'slide1.png' height="450px"></img>
</footer>


This is the link to the shiny app: https://lalang.shinyapps.io/dataproduct/

---
## Wind Measurement classified by Day
To plot the wind measurement on daily basis, we use rCharts

```r
library(UsingR)
require(rCharts)
require(knitr)
data(airquality)

p1 <- rPlot(Wind~Day, data=airquality, color="Month",type="point",size = list(const = 3))
         p1$addParams(width = 600, height = 400, dom = 'chart1',
                     title = " Wind Scatter Plot on regular daily basis")
         p1$guides(x = list(title = "", min = 0,max = 32 ))
         p1$guides(y = list(title = "", max = 22))
```

---

## Wind Measurement classified by Day(cont)

This is the link to the shiny app: https://lalang.shinyapps.io/dataproduct/

---

## Data Source Interaction 
Data manipulation can be done in R while navigating the data source tab.
<footer class = 'logo'>
  <img src = 'slide3.png' height="400px"></img>
</footer>

This is the link to the shiny app: https://lalang.shinyapps.io/dataproduct/
