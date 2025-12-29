# 🚀 Atmosphere Update: Version 3.0 (Ultimate Edition)

This major update transforms the project from a minimal weather tool into a fully immersive, "Atmosphere-focused" weather station. Below is the breakdown of the architectural evolution.

## 🏗️ 1. Original Structure (Legacy V2)
The original project was a lightweight, single-file weather application built with Vanilla JS.
*   **Core Logic:** It utilized direct fetching from the Open-Meteo API to display current weather and basic daily forecasts.
*   **UI/UX:** A minimalist card-based layout with static solid/gradient backgrounds.
*   **Functionality:**
    *   Direct DOM manipulation for updating values.
    *   Automatic loading of a default city (e.g., Tehran) on startup.
    *   Basic search functionality via a simple input field.
*   **Verdict:** It served as a solid, functional foundation and a great example of clean API integration.

---

## ⚡ 2. Version 3.0 Architecture (The Overhaul)
Version 3.1 builds upon the original logic but refactors the entire frontend and introduces a dynamic engine for visuals.

### 🎨 UI/UX Redesign (Glassmorphism)
*   **Glass Engine:** Replaced solid cards with a premium **Glassmorphism** design (blur filters, translucent borders, and shadows) to create depth.
*   **Typography:** Migrated to **Poppins** font for a modern, global look.
*   **Mobile-First Search:** Implemented a full-screen search overlay to improve usability on mobile devices.
*   **Landing Screen:** Introduced a "Welcome Screen" to prevent auto-loading, giving users control from the start.

### 🧠 Core Logic Upgrades
*   **Timezone Awareness:** The app now calculates and displays the **Local Time** of the searched city (not the user's device time), adding a layer of realism.
*   **Data Expansion:**
    *   Added **Hourly Forecast (24h)** with horizontal scrolling.
    *   Added **Humidity**, **Wind Speed**, and **High/Low** temperatures.
    *   Visual "Temperature Bars" added to the 7-day forecast.

### 🌦️ Dynamic Atmosphere Engine
This is the heart of V3. The background and visuals now react to data:
1.  **Smart Gradients:** The background gradient shifts smoothly based on two factors:
    *   **Time of Day:** (Day/Night cycles).
    *   **Weather Condition:** (Clear, Cloudy, Rain, Snow).
2.  **HTML5 Canvas Particle System:**
    *   Instead of heavy GIFs/Videos, we use lightweight JavaScript Canvas to render **Rain** and **Snow**.
    *   **Rain:** Fast, slanted linear drops.
    *   **Snow:** Slow, drifting circular particles.
    *   *Optimization:* The animation loop stops automatically when the weather is clear to save battery/performance.

### 🛠️ Technical Refactoring
*   **Error Handling:** Improved `try/catch` blocks for network requests and geolocation errors.
*   **Loader:** Added a CSS spinner during API fetch states.
*   **Footer:** Added a credit pill linking back to the original author.
## 🌟 Key Features

*   **iOS-Inspired Design:** Clean typography (SF Pro style), frosted glass effects, and a minimalist interface.
*   **Real-Time Data (Powered by Open-Meteo):**
    *   Temperature & Real Feel
    *   Humidity & Wind Speed
    *   Atmospheric Pressure (New!)
    *   Hourly & 7-Day Forecast
*   **Dynamic Atmosphere:**
    *   Background gradients change based on weather conditions (Clear, Rain, Snow, Storm).
    *   **Parallax Effect:** Background moves subtly with your mouse cursor for a 3D feel.
*   **Smart Geocoding:** Search for any city worldwide with auto-focus and error handling.
*   **No API Key Required:** Plug and play! Uses the free Open-Meteo API.

## 🛠️ Tech Stack

*   **HTML5 Canvas** (Particle System & Animation)
*   **CSS3** (Grid, Flexbox, Backdrop-Filter, Keyframes)
*   **JavaScript (ES6+)** (OOP, Async/Await, Fetch API)
*   **API:** [Open-Meteo](https://open-meteo.com/)

## 📸 Screenshots
### v3.0 (Ultimate Edition)

### v2.0 (New Interface)
Soon ...

### v1.0 (Legacy Design)
![1](https://github.com/user-attachments/assets/895edef7-4a43-4e00-b097-16d43036c087)
![2](https://github.com/user-attachments/assets/22fe98f5-4b3d-43f1-aba9-9a5a3ca01521)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
