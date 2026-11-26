# IgnisAI

I started IgnisAI as my Cal State Fullerton capstone after the January 2025 Eaton and Palisades fires. I wanted to see whether publicly available data could help fire crews answer a practical question: where might a fire spread next, and what’s in its path?

**[Explore the live map](https://ignisai-frontend.onrender.com/dashboard)**

![IgnisAI incident map across the western United States](screenshots/live-incident-map.jpg)

The map shows reported fire perimeters and NASA satellite detections. A Python forecast service combines recent detections with NOAA weather, terrain, and fuel data to estimate how a fire might spread over time. The forecast is shown separately from what’s been observed.

To see an example, open **Past fires → Palisades Fire**. Forecasts are advisory, not official perimeters or evacuation guidance.

The source code and model weights are private.
