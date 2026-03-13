# ⚡ HiRES Energy Monitor

A mobile-first, glassmorphism web dashboard designed to monitor and simulate a Hybrid Renewable Energy System (Solar & Wind). 

## 🚀 Overview
HiRES provides a real-time interface for tracking renewable energy generation, battery storage, and power consumption. It features a built-in simulation engine that adjusts power generation based on live weather data and syncs system telemetry to the cloud for IoT monitoring.

## ✨ Key Features
* **Real-Time Weather Integration:** Fetches live temperature, wind speed, cloud cover, and solar irradiance using the Open-Meteo API.
* **Smart Simulation:** Dynamically calculates solar and wind generation based on weather conditions and manages a simulated 10kWh Li-ion battery.
* **IoT Cloud Sync:** Automatically pushes live telemetry data (solar, wind, battery percentage, and load) to ThingSpeak every 20 seconds.
* **Interactive Analytics:** Visualizes power generation history using dynamic charts.
* **System Controls:** Allows users to manually prioritize energy sources, toggle AC/DC loads, and simulate day/night conditions.

## 🛠️ Tech Stack
* **Frontend:** HTML5, Vanilla JavaScript
* **Styling:** Tailwind CSS (via CDN), custom Glassmorphism CSS
* **Icons & Charts:** FontAwesome, Chart.js
* **APIs:** Open-Meteo (Weather), ThingSpeak (Cloud/IoT)

## 💻 How to Run
Because this project relies entirely on client-side web technologies and public CDNs, there are no complex installation steps, servers, or dependencies required!

1. Download or clone this repository.
2. Open the `index.html` file directly in any modern web browser (Chrome, Edge, Safari, Firefox).
3. The dashboard will automatically fetch local weather data and begin the system simulation.

## ⚙️ Configuration (Optional)
If you want to connect the dashboard to your own ThingSpeak channel:
1. Open `index.html` in a text editor.
2. Locate the `CLOUD_CONFIG` object.
3. Replace the `channelID`, `writeKey`, and `readKey` with your own ThingSpeak credentials.
