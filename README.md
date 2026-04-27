# 🌱 SoilScope

> **Monitor your soil, water, and air conditions — in real time.**

SoilScope is a lightweight environmental monitoring dashboard built for farmers, researchers, and environmentalists. It fuses satellite-derived vegetation indices, live weather data, and geolocation to deliver hyperlocal soil and environmental health insights — right down to the village level.

---

## 📸 Preview

![SoilScope Dashboard](./screenshot.png)

---

## ✨ Features

- **Soil Health Monitoring** — Real-time soil moisture readings and NDVI (Normalized Difference Vegetation Index) tracking
- **Water Quality Assessment** — Evaluates water safety for irrigation purposes
- **Air Quality Index** — Live air condition monitoring with status indicators
- **Interactive Map** — Leaflet.js-powered map with clickable location pins showing pH and NDVI data
- **Live Weather Integration** — Powered by Open-Meteo API; shows temperature, humidity, wind speed, rainfall, and conditions
- **Hyperlocal Geolocation** — Resolves coordinates to village/taluk/district level
- **CropLens AI** — AI-powered crop analysis module *(in development)*
- **Pest Patrol** — Pest detection and alert system *(in development)*
- **Market Prices** — Live agricultural commodity prices *(in development)*
- **Precipitation Radar** — Visualize upcoming rainfall patterns
- **Multilingual Support** — English and regional language support

---

## 🗺️ How It Works

1. **Enter or detect your location** using the search bar or "My Location" button
2. **Fetch Data** pulls satellite NDVI, soil moisture, and weather for that coordinate
3. The dashboard updates with **Soil Health**, **Water Quality**, and **Air Quality** cards
4. Drill deeper with **Detailed Analysis** for full sensor breakdowns
5. **Save** locations for recurring monitoring

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML / CSS / JavaScript (or React) |
| Maps | Leaflet.js + OpenStreetMap |
| Weather API | Open-Meteo (free, no key required) |
| Satellite Data | NASA MODIS / Sentinel via NDVI APIs |
| Geolocation | Browser Geolocation API + Reverse Geocoding |
| AI Module | Claude API *(CropLens AI)* |

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ (if using a bundler)
- A modern browser

### Installation

```bash
git clone https://github.com/yourusername/soilscope.git
cd soilscope
npm install
npm run dev
```

Or simply open `index.html` in your browser if it's a vanilla JS project.

---

## 📡 API Configuration

Create a `.env` file in the root:

```env
VITE_WEATHER_API=https://api.open-meteo.com/v1/forecast
VITE_NDVI_API=your_ndvi_api_endpoint
VITE_GEOCODE_API=your_reverse_geocoding_key
```

---

## 📊 Data Sources

| Data Type | Source | Refresh Rate |
|---|---|---|
| Weather | Open-Meteo | Live |
| NDVI Index | NASA MODIS / Sentinel-2 | Daily |
| Soil Moisture | Satellite + Sensor Fusion | Daily |
| Air Quality | OpenAQ / WAQI | Hourly |
| Water Quality | Derived model | On fetch |

---

## 🔬 Research Context

SoilScope was developed as part of an environmental research project exploring whether **low-cost, open-source remote sensing tools** can provide actionable soil health data to smallholder farmers in India — without expensive hardware.

Key research questions:
- How accurately can satellite NDVI predict ground-level soil moisture at village scale?
- Can real-time environmental dashboards meaningfully reduce crop stress response time?
- What is the minimum viable data resolution for farm-level irrigation decisions?

> Validation fieldwork ongoing across multiple soil regions in India.

---


## 🛣️ Roadmap

- [x] Live weather integration
- [x] NDVI + soil moisture display
- [x] Interactive map with location pins
- [ ] CropLens AI — crop disease detection from image
- [ ] Pest Patrol — alert system for pest outbreaks
- [ ] Market Prices — live mandi rates
- [ ] Offline mode for low-connectivity rural areas
- [ ] Mobile app (React Native)
- [ ] Ground truth validation dataset

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repo
2. Create your branch (`git checkout -b feature/your-feature`)
3. Commit changes (`git commit -m 'Add your feature'`)
4. Push to branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---



## 👤 Author

**Araadh311**  
Environmental Research Project — 2025  
Built with the goal of making precision agriculture accessible to every farmer.

---

> *"The soil is the great connector of lives, the source and destination of all."*  
> — Wendell Berry
