# Flood Monitoring Tool

## Project Overview
The Flood Monitoring Tool is a web-based application that enables users to monitor real-time flood data from various measurement stations provided by the Environmental Agency's public API. Users can select an individual station from a list and view a line graph displaying the station’s readings over the past 24 hours, along with a corresponding data table for detailed inspection.

This tool aims to provide an intuitive and user-friendly interface for real-time flood data visualization, helping users, researchers, and decision-makers to easily track water levels and respond proactively to flood risks.

## Features
- Dynamic dropdown list of flood measurement stations fetched from the Environmental Agency’s API.
- Interactive line chart showing real-time readings of the selected station for the last 24 hours.
- Accompanying data table presenting exact readings with timestamps.
- Responsive and clean user interface styled with CSS.
- Uses Chart.js for smooth, animated graph rendering.
- Time axis uses date-fns adapter for accurate date/time formatting.

## Technologies Used
- HTML5, CSS3, JavaScript (ES6)
- Chart.js (for chart visualization)
- Environmental Agency Flood Monitoring API (https://environment.data.gov.uk/flood-monitoring/)
- date-fns (for date handling and formatting)

## Setup and Usage
1. Clone the repository or download the source code.
2. To avoid CORS issues with API requests, serve the files locally using a simple HTTP server:
   ```bash
   python -m http.server 8000

3. Select a measurement station from the dropdown list to load its readings.
4. The line graph and table will update dynamically with the station’s data from the last 24 hours.

## Notes
Due to browser security policies (CORS), the tool needs to be served over HTTP locally or deployed on a web server.
The Environmental Agency API availability and data accuracy depend on their server and sensors.
