# ⚡️ Weather Widget: Real-Time Data & Immersive Visuals

This project is a clean, modern weather widget built using Vanilla JavaScript and Tailwind CSS. It is designed to be highly stable and uses the official OpenWeatherMap API for accurate, real-time current weather and forecast data.

This widget was created to demonstrate skills in asynchronous data handling, responsive design, and dynamic CSS manipulation (visual weather effects).

## ✨ Key Features

* **Real-Time Data:** Fetches live weather, temperature, humidity, wind, sunrise/sunset times, and pressure.
* **Search Functionality:** Allows searching for any city via the OpenWeatherMap Geocoding API.
* **Dynamic Visuals:** Includes immersive, animated visual effects (rain, snow, wind) that dynamically change based on the live weather data (though currently disabled for manual use).
* **Stable UI:** Uses asynchronous JavaScript structured within `window.onload` to ensure the UI remains functional even during API connection delays.
* **Modern Aesthetic:** Utilizes Tailwind CSS for a clean, glassmorphism-inspired design.

## ⚙️ Installation & Setup (Production Ready)

This is a static HTML/CSS/JS project and **does not require Node.js or a backend server to run**.

### 1. File Structure

Ensure your project directory contains the following two files:
/Weather-App/ ├── index.html // Main widget structure └── script.js // Core logic, API calls, and animations └── style.css // All compiled CSS/Tailwind utilities

### 2. API Key Configuration (Crucial Step)

To fetch live data, you must insert your OpenWeatherMap API key into the JavaScript file.

1.  Get your free API key from [OpenWeatherMap](https://openweathermap.org/api).
2.  Open **`script.js`** in your code editor.
3.  Find the following line (around the configuration section) and replace the placeholder value:

    ```javascript
    const WEATHER_API_KEY = '################################'; // <--- REPLACE THIS WITH YOUR API VALUE
    ```

### 3. Running the App

To view the widget, simply double-click the **`index.html`** file in your web browser.

## 💻 Technical Details

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Data Fetching** | Vanilla JavaScript (`fetch`) | Handles asynchronous requests to the API. |
| **APIs Used** | OpenWeatherMap (`/weather`, `/forecast`) | Provides real-time meteorological data. |
| **Geocoding** | OpenWeatherMap Geocoding API | Converts city names to latitude/longitude coordinates for data lookup. |
| **Styling** | Tailwind CSS (Compiled) | Utility-first styling for the modern aesthetic. |
| **Animation** | Pure CSS Keyframes & JS | Used for the rain, snow, and gentle UI effects. |

## 💡 Note on Stability

The initial JavaScript logic is structured using `window.onload` to prevent instability. If you face a **401 Unauthorized** error upon initial load, your API key is either incorrect or is still in the 2-hour activation period required by OpenWeatherMap.

---
*Created by Sai Hanumanthavajjala.*
