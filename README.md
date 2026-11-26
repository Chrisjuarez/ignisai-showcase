# IgnisAI

IgnisAI is a wildfire map for the western United States. It brings together active incidents, reported perimeters, satellite hotspots, and fire-weather alerts. Advisory spread forecasts are shown separately from observed fire data.

**[Open the live map](https://ignisai-frontend.onrender.com/dashboard)** · No account needed to explore.

![IgnisAI live map with wildfire incident markers across the western United States](screenshots/live-incident-map.jpg)

## Why I Built It

I started IgnisAI as a capstone project to explore how wildfire data from different sources could fit on one map. I wanted to make it easier to compare what has been observed with where a model suggests a fire might spread.

## How It Works

A React and Mapbox dashboard reads incident, perimeter, and alert data from an Express API. A separate Python service uses recent satellite detections, weather, terrain, and fuel data to run a PyTorch ConvLSTM model. The map displays the results as a timeline, separate from reported perimeters and hotspots.

## Try a Historical Forecast

Open **Past fires** and select **Palisades Fire**. Use the timeline to step through the advisory forecast and compare it with observed layers where available.

**For situational awareness only.** Forecasts are not official fire perimeters or evacuation guidance. Follow local authorities for emergency instructions.

This repository is a public showcase. The application source code and model weights are private.
