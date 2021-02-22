# ** Chart.js
** Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.**

## How to use charts?

- first download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page.
- Drawing a line chart.
- write a script that will retrieve the context of the canvas
- create our data in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart.
- Drawing a pie chart.
- Next we need to get the context and to instantiate the chart.
- create the data: this data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for sections.
- then add your option: these options do two things: remove the stroke from the segments then animate the scale of the pie so that it zooms out from nothing.
- Drawing a bar chart Finally: add  a bar chart to the page ,the syntax for the bar chart is very similar to the line chart we already added. First we add the canvas element Next we retrieve the element and create the graph then we add in the bar chart’s data.
- chose to use RGBA to specify colors which allows to add transparency.
