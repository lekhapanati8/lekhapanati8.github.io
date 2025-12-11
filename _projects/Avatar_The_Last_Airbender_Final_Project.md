---
name: Journeying through the world of Avatar The Last Airbender
tools: [Python, HTML, vega-lite]
image: https://i.pinimg.com/originals/c4/88/d3/c488d3700be287c6a1f229ccd9c26e8a.png
description: This is Lekha's submission for FP 3.1.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Journeying through the world of Avatar: The Last Airbender

### Created by Lekha Panati

<vegachart
    schema-url="{{ site.baseurl }}/assets/json/avatarheatmapfinal.json"
    style="width: 100%">
</vegachart>

<vegachart
    schema-url="{{ site.baseurl }}/assets/json/avatarbarfinal.json"
    style="width: 100%">
</vegachart>

My primary visualization is a heatmap showing how often major locations are mentioned across the episodes of _Avatar: The Last Airbender_. Each row represents a different place in the Avatar world, such as the Southern Water Tribe, Omashu, or Ba Sing Se, and each column represents an episode. The color of each cell indicates how frequently that location is mentioned. Darker shades highlight episodes where a place plays an important narrative role, while lighter shades show moments where it is not discussed as much. This heatmap helps viewers quickly see how the story moves from one region to another throughout the series, revealing patterns such as early activity around the Southern Air Temple or sustained attention on Ba Sing Se during major plot arcs.

To help viewers better understand the physical layout of these locations, our first contextual visualization is a map of the top thirty places mentioned in the transcripts. Using fan-curated coordinate data, each location is plotted on the world map with a labeled marker. This map translates the heatmap’s abstract patterns into real geography. When a cluster of episodes focuses on the Earth Kingdom, for example, the viewer can refer back to the map and recognize the shifts in region and setting. This makes it easier for newcomers to visualize the flow of the story world and understand how the characters move across vast distances.

Our second contextual visualization is a bar chart showing the bending arts that appear most often in the dialogue. This adds narrative context by highlighting which elemental abilities are most prominent in each book. Unsurprisingly, earthbending is emphasized in Book 2: Earth, while firebending becomes more common in Book 3: Fire. This chart helps readers connect character development and plot progression to the themes of the show, reinforcing the central idea that Aang must master all four elements to restore balance.

Together, these three visualizations give a clear overview of how the world, characters, and themes evolve throughout the series. They allow viewers new to data analysis to explore the show’s structure through both geographic and narrative lenses.

**I created all visualizations, including contextual :)**
