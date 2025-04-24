# recent-earthquakes
A visualization of recent earthquake data pulled 4/24/2025.

This repository is an extension from exercise 16-8 of the Python Crash Course by Eric Matthes. 

The prompt for Exercise 16-8 is as follows: *You can find data files containing information about the most recent earthquakes over 1-hour, 1-day, 7-day and 30-day periods online. Download a dataset and create a visualization of the most recent earthquake activity.*

While the general process was learned throughout the chapter, this exercise required readers to pull new data and adjust for issues that may occur when working with a new data set. Issues that were personally faced with a new dataset included the following:
- Issues with encoding: Resolved by explicitly stating 'utf-8' when opening the file.
- Negative magnitudes causing calculation issues: Resolved by adding an if statement to only pull data for positive value magnitudes.

The data used for this project was pulled on 4/24/2025 from https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php. The data consisted of all earthquakes from the past 7 days.

This repository consists of the following files:
- *recent_earthquakes_plot.py* - The main executable file for this project. This file contains all necessary code to extract the JSON data and plot it on a world map using the plotly library.
- *recent_eq_data.json* - The data used for this project.
- *recent_global_earthquakes.html* - A sample output one would expect if running this program.
