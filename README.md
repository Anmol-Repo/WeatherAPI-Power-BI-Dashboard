# WeatherAPI Power BI Dashboard 🌤️

An interactive Power BI dashboard that visualizes real-time and forecast weather data using the WeatherAPI.com service.  
The project demonstrates API integration, JSON data transformation, and dashboard design with actionable insights.

## Screenshots
![weather dashboard 1 _page-0001](https://github.com/user-attachments/assets/f0acd784-5690-49ae-a968-15bf6df0d980)
![weather dashboard2_page-0001](https://github.com/user-attachments/assets/462f8034-40ac-4d09-96b7-f50554b55244)
![weather dashboard 3 pdf_page-0001](https://github.com/user-attachments/assets/1555e964-babd-4371-a39f-e07531fcd4b9)



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
