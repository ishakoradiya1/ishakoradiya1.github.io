---
name: Homework 5
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/cars.png
description: Homework 5's charts and discussion.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 5

Chart 1:
<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.json" style="width: 100%"></vegachart>

For my first visualization, I chose a bar chart that visualizes the frequency of UFO sightings categorized by shape and country. Specifically, each bar represents a different UFO shape and the height of the bar corresponds to the number of sightings for that shape based on country. The color scheme was chosen so that users can visually see the difference between the UFO sightings for the various countries so that it is readable. Additionally, the chart uses categorical encoding on the x-axis (UFO shapes) and quantitative encoding on y-axis (count of sightings). Similarly, for the color of the bars it is encoded as nominal as we are looking at countries. Overall, there were not any major transformations apart from sampling 5000 records from the dataset in order to make it more manageable for visualization. 

Plot 2:
<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.json" style="width: 100%"></vegachart>

For my second visualization, I chose a scatterplot that visualizes the relationship between the duration of UFO sightings (in seconds) and their latitude, with each point representing a UFO sight. Additionally, the color of the points on the plot indicates the shape of the UFO that was sighted. The plot uses quantitative encoding for Duration on the x-axis and latitude is encoded on the y-axis. Similarly, the color of the points is based and encoded based on the shape variable which helps see how the UFO types differ. For interactivity, users can hover over the specific points to view information about a specific point (UFO sight) to see the duration, latitude, and shape and users can also use a dropdown to group the UFO types based off of a specific shape. This was chosen because without it is difficult to see what many of the points' exact values are and users can now filter based on the specific UFO type in regards to shape and see clearly the duration of each shape group

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="{{ site.baseurl }}/assets/json/ufo-scrubbed-geocoded-time-standardized-00.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ishakoradiya1/ishakoradiya1.github.io/blob/main/python_notebooks/workbook.ipynb" text="The Analysis" %}
</div>
