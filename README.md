# WeatherAPI Power BI Dashboard 🌤️

## Overview
An interactive Power BI dashboard that visualizes real-time and forecast weather data using the WeatherAPI.com service.  
The project demonstrates API integration, JSON data transformation, and dashboard design with actionable insights.

## Features
- Integrated WeatherAPI.com JSON data into Power BI using the Web API connector
- Transformed and modeled data with Power Query and DAX
- Visualizations:
  - Temperature & humidity trend lines
  - KPI cards for current conditions
  - City-wise weather comparison
  - Map view of multiple cities
- Refreshable dataset for real-time updates

## Setup Instructions
1. Sign up at [WeatherAPI.com](https://www.weatherapi.com/) and get your API key.
2. Example request for 5-day forecast:
```

[https://api.weatherapi.com/v1/forecast.json?key=YOUR\_API\_KEY\&q=London\&days=5](https://api.weatherapi.com/v1/forecast.json?key=YOUR_API_KEY&q=Dehradun&days=5)

```
3. In Power BI:
- Go to **Get Data → Web**
- Paste the API URL with your key
- Parse JSON in Power Query and transform data
- Build visuals and KPIs

## Repository Structure
```

weatherapi-powerbi-dashboard/
│
├── weather\_dashboard.pbix        # Power BI project file
├── data/                         # (Optional) Sample CSV export of API data
├── screenshots/                  # Dashboard previews
│   ├── main\_dashboard.png
│   └── forecast\_trend.png
└── README.md

```

## Screenshots
*(Dashboard screenshots will be added here shortly )*

## Files
- `weather_dashboard.pbix` → Main Power BI dashboard
- `data/` → Optional CSVs for sample weather data
- `screenshots/` → Dashboard preview images

## Insights
- Quickly track city-level weather patterns
- Compare forecasts across multiple regions
- Enable decision-making based on live weather updates
```

---
