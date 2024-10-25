# Real-Time Weather Monitoring System

## Overview

This project is a **Real-Time Weather Monitoring System** that fetches weather data from the **OpenWeatherMap API**. It provides real-time weather information, 5-day forecasts, and features temperature conversion between Celsius, Fahrenheit, and Kelvin. It also calculates daily weather summaries such as average, max, and min temperatures and visualizes temperature trends using Chart.js.

## Features

- **API Integration**: Connects to the OpenWeatherMap API to fetch real-time weather data.
- **Weather Summaries**: Provides daily forecasts with max, min, and average temperatures.
- **Temperature Conversion**: Allows conversion between Celsius, Fahrenheit, and Kelvin based on user preference.
- **Daily Weather Summary**: Calculates daily averages, max, and min temperatures, and determines the dominant weather condition.
- **Additional Data**: Displays humidity and wind speed.
- **5-Day Forecast**: Shows weather for upcoming days, updated every 3 hours.
- **Threshold Alerts**: Allows users to set temperature thresholds and triggers alerts when the thresholds are breached.
- **Data Visualization**: Visualizes temperature trends over time using Chart.js.

## Fulfillment of Requirements

- **Data Source**:
  - Continuously retrieves weather data from the OpenWeatherMap API for major metros in India (Delhi, Mumbai, Chennai, Bangalore, Kolkata, Hyderabad).
  - Processes weather data such as temperature, humidity, wind speed, and main weather conditions.
  
- **Processing and Analysis**:
  - Calls the API at configurable intervals (e.g., every 5 minutes).
  - Converts temperature values from Kelvin to Celsius or Fahrenheit.

- **Rollups and Aggregates**:
  - **Daily Weather Summary**:
    - Rolls up daily weather data and computes average, maximum, minimum temperatures, and the dominant weather condition.
    - Stores daily summaries in persistent storage for further analysis.
  
  - **Threshold Alerts**:
    - Users can define custom temperature thresholds.
    - Alerts are triggered if the temperature exceeds the threshold for two consecutive updates.
  
  - **Visualizations**:
    - Displays temperature trends and daily summaries using a line chart.

## Design Highlights

- **Modular Structure**: Separate modules handle API connection, data processing, and UI rendering.
- **Configurable**: Users can customize temperature units and forecast intervals.
- **Easily Extendable**: Additional weather parameters can be incorporated with minimal effort.

## Requirements

- **Minimum screen resolution**: 1070x680
- **Node.js**: Required for running a local server (optional).

## Setup

### Prerequisites

- Install [Node.js](https://nodejs.org/en/) on your system.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/Real-Time-Weather-App.git
   ```

2. **Navigate to the project folder**:
   ```bash
   cd Real-Time-Weather-App
   ```

3. **Install Dependencies**:
   ```bash
   npm install
   ```

4. **Run the server**:
   ```bash
   npm install http-server -g
   http-server -p 8080
   ```

   Alternatively, you can open `index.html` directly in a browser for simple testing.

## Usage

- Enter a city name in the search bar to fetch real-time weather data.
- Use the dropdown menu to switch between Celsius, Fahrenheit, and Kelvin.
- View daily weather summaries, along with detailed humidity and wind speed data.

## Additional Information

- The project can be extended to include additional weather parameters like atmospheric pressure or UV index, which are available via the OpenWeatherMap API.
- You can also configure additional thresholds for weather alerts or customize the alerting logic.

---



