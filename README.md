# 🌤️ Weather Pro

> A sleek, real-time weather dashboard powered by the **WeatherAPI.com** REST API — built with pure HTML, CSS & JavaScript.

![Weather Pro Banner](https://img.shields.io/badge/API-WeatherAPI.com-blue?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---
<!--
## 🚀 Live Demo

> 🔗 **[View Live →](https://atharvathawkar.github.io/weather-pro)** *(update link after deployment)*
-->
---

## 📸 Preview

| Sunny ☀️ | Rainy 🌧️ | Cloudy ⛅ |
|----------|----------|----------|
| *Golden gradient background* | *Blue gradient background* | *Dark gradient background* |

> The background theme **dynamically changes** based on current weather conditions!

---

## ✨ Features

- 🔍 **City Search** — Search any city worldwide by name or press `Enter` to search
- 🌡️ **Current Weather** — Real-time temperature, weather condition, and icon
- 💧 **Detailed Stats** — Feels Like temperature, Humidity %, and Wind Speed (km/h)
- 📅 **3-Day Forecast** — Upcoming weather with daily average temperature and condition
- 🎨 **Dynamic Backgrounds** — Gradient theme changes automatically based on weather (sunny, rainy, cloudy, snowy)
- 📍 **Default Location** — Auto-loads weather for **Pune, India** on startup
- 📱 **Fully Responsive** — Works seamlessly on mobile, tablet, and desktop

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| **HTML5** | Markup & page structure |
| **CSS3** | Glassmorphism UI, animations, responsive layout |
| **JavaScript (ES6+)** | Async API calls, DOM manipulation, dynamic rendering |
| **WeatherAPI.com** | Live weather data (current + forecast + AQI + alerts) |
| **Google Fonts (Poppins)** | Typography |

---

## 📡 API Reference

This project uses the **[WeatherAPI.com](https://www.weatherapi.com/)** REST API.

**Endpoint used:**
```
GET https://api.weatherapi.com/v1/forecast.json
    ?key=YOUR_API_KEY
    &q={city}
    &days=3
    &aqi=yes
    &alerts=yes
```

**Data consumed:**
- `location.name` / `location.country` / `location.localtime`
- `current.temp_c` / `current.feelslike_c` / `current.humidity` / `current.wind_kph`
- `current.condition.text` / `current.condition.icon`
- `forecast.forecastday[].day.avgtemp_c` / `condition.text` / `condition.icon`

---

## ⚙️ Getting Started

### Prerequisites
- A free API key from [WeatherAPI.com](https://www.weatherapi.com/signup.aspx)
- A modern browser (Chrome, Firefox, Edge, Safari)

### Installation

**1. Clone the repository**
```bash
git clone https://github.com/AtharvaThawkar/weather-pro.git
cd weather-pro
```

**2. Add your API key**

Open `index.html` and replace the API key on this line:
```javascript
const API_KEY = "your_api_key_here";
```

**3. Run the project**

Simply open `index.html` in your browser — no build tools or server required!
```bash
# Or use VS Code Live Server for a better dev experience
```

---

## 📁 Project Structure

```
weather-pro/
│
├── index.html        # Main HTML file (UI + JS logic all-in-one)
└── README.md         # Project documentation
```

---

## 🎨 UI Highlights

- **Glassmorphism design** — backdrop blur, semi-transparent cards
- **Smooth transitions** — background color shifts on weather change (0.8s transition)
- **Responsive grid** — stats and forecast cards reflow cleanly on smaller screens
- **Hover effects** — subtle scale animation on the search button

---

## 🔮 Future Improvements

- [ ] Toggle between **Celsius / Fahrenheit**
- [ ] **Geolocation support** — auto-detect user's current location
- [ ] **Air Quality Index (AQI)** display using existing API data
- [ ] **Weather alerts** section for severe conditions
- [ ] **Hourly forecast** chart using Chart.js
- [ ] Store **recently searched cities** using localStorage

---

## ⚠️ Important Note

> This project uses a **client-side API key** which is exposed in the source code. This is acceptable for learning/portfolio projects. For production use, the API call should be routed through a **backend server** (e.g. Node.js + Express) to keep the key secure.

---

## 👨‍💻 Author

**Atharva Pramod Thawkar**
- 🎓 Final Year B.E. IT — SIPNA College of Engineering, Amravati
- 💼 Aspiring MERN Stack Developer | Open to Opportunities
- 🔗 [GitHub](https://github.com/AtharvaThawkar) · [LinkedIn](https://linkedin.com/in/atharva-t-8b6620261) · [LeetCode](https://leetcode.com/u/Atharva_Thawkar/)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ **If you found this project useful, please consider giving it a star!** It helps a lot 🙏
