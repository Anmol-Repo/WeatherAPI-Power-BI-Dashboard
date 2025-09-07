# WeatherAPI Power BI Dashboard 🌤️

An interactive Power BI dashboard that visualizes real-time and forecast weather data using the WeatherAPI.com service.  
The project demonstrates API integration, JSON data transformation, and dashboard design with actionable insights.


## Screenshots & GIFs
![weather dashboard 1 _page-0001](https://github.com/user-attachments/assets/f0acd784-5690-49ae-a968-15bf6df0d980)
![weather dashboard2_page-0001](https://github.com/user-attachments/assets/462f8034-40ac-4d09-96b7-f50554b55244)
![weather dashboard 3 pdf_page-0001](https://github.com/user-attachments/assets/1555e964-babd-4371-a39f-e07531fcd4b9)

![Dashboard_1080p](https://github.com/user-attachments/assets/f2caf54f-e94a-46e8-a8c3-50164ffe80ec)



## ✨ Features
- Integrated WeatherAPI.com JSON data into Power BI using the Web API connector
- Transformed and modeled data with Power Query and DAX
- Visualizations:
  - Temperature & humidity trend lines<br>
  - KPI cards for current conditions<br>
  - City-wise weather comparison<br>
  - Refreshable dataset for real-time updates<br>

## ✅ Prerequisites (exact)

1. **WeatherAPI.com** account (free *or* paid) **API key required**.
2. **Power BI Desktop** (latest stable).
3. Familiarity with **Power Query (M)** & **DAX**.

---
## What this project shows

End-to-end API → Power Query → star-schema → DAX → interactive PBIX.<br>
Real-world JSON shaping: nested record expansion, type-casting, error handling, and column pruning for performance.<br>
Reusable parameterization: API_KEY and CityList to make the report repeatable and production-friendly.<br>
Visuals focused on decision-making: KPI cards, 7-day trends, and city comparisons.<br>

## 🛠️ Setup (3 quick steps)

1. **Create parameters:** `API_KEY` (Text) and `CityList` (Table/CSV).
2. **Connect:** Get Data → **Web** → use parametrized URL `https://api.weatherapi.com/v1/forecast.json?key=API_KEY&q=City&days=5&aqi=yes`.
3. **Transform:** Use an M function to call the API per city → expand `location`, `current`, `forecast` → set types → load into `City`, `CurrentConditions`, `Forecast` tables.

## ⚙️ Quick production notes

* **Do not** hardcode API keys. Use parameters or Key Vault.<br>
* Handle rate-limits and HTTP errors (try/otherwise in M).<br>
* Normalize timestamps to city local time.<br>
* Schedule refresh in Power BI Service; configure gateway if using on-prem.<br>

## 📁 Repo (suggested)

```
weatherapi-powerbi-dashboard/
├─ weather_dashboard.pbix
└─ screenshots/         # PNGs / GIFs 
```



