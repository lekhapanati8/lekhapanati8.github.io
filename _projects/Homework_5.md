---
name: Homework 5
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# UFO Sighting Plots

<vegachart schema-url="{{ site.baseurl }}/assets/json/line.json" style="width: 100%"></vegachart>

For my first visualization, I generated a line chart that displays the total number of UFO sightings per year across the United States. This graph provides a high-level view of how UFO reporting frequency has changed over time. A line mark was selected because line charts naturally reveal trends, increases, and decreases in temporal data.

To build the plot, I extracted the year from the ufosDS date column and filtered the dataset so only the rows with sightings in the US were included (df_us). I then computed an aggregation to obtain the total number of sightings for each year. The year is encoded on the x-axis and treated as an ordered field, while the total count is encoded on the y-axis. I avoided adding a color encoding because there is no additional variable needing differentiation. 

Even without interactivity, this line chart is a useful, clear summary of long-term UFO reporting trends.

<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/bar.json" style="width: 100%"></vegachart>

This plot displays the number of UFO sightings in each US state for a single selected year. The purpose is to see how the geographic distribution of sightings has changed over time. I chose to configure a bar chart as the visualization showcases counts across discrete categories (states). 

For data preprocessing, I used the same df_us dataset as the line chart, which contains only reports from the United States. The state variable is encoded on the x-axis as a nominal field, and Altair’s count() aggregate is used on the y-axis to compute the number of sightings per state.

The interactivity in the bar chart comes from a year slider. This slider updates the visualization by filtering each data entry's year to the current slider value. This interactive filtering makes the visualization more engaging and more effective for identifying temporal patterns.

## Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/ufo-scrubbed-geocoded-time-standardized-00.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/lekhapanati8/lekhapanati8.github.io/blob/9e5aafe1c8256ee00da83c01f158ee2bdc66521d/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
