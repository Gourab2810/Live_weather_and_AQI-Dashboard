# 🌤️ Weather & AQI Dashboard — Power BI

[Dashboard Preview](<img width="1322" height="744" alt="Weather and AQI Dashboard" src="https://github.com/user-attachments/assets/343e7989-1b80-4d63-9a46-099ebd0cfec8" />)

##  Overview

An interactive **Weather & Air Quality Index (AQI) Dashboard** built in **Power BI**, 
fetching live data from **WeatherAPI.com**. The dashboard provides real-time weather 
conditions, a 7-day forecast, air quality metrics, and other key weather KPIs — 
all wrapped in a sleek dark mode with an orange gradient theme.



## 🔗 Data Source

- **API:** [WeatherAPI.com](https://www.weatherapi.com/)
- Live weather data was fetched from the API and imported directly into Power BI
- Data was then cleaned, transformed, and modeled into structured tables



##  Data Cleaning & Modeling

After importing the raw API data, the following steps were performed:

- Cleaned and transformed raw JSON/API response data in **Power Query**
- Structured the data into **3 separate tables:**

| Table | Description |

| `Current Weather` | Real-time weather data for selected city |
| `Forecast Day` | Day-wise forecast data for 7 days |
| `Forecast Hours` | Hour-wise forecast breakdown |



##  Dashboard Features & KPIs

### City Selector
- Toggle between **Bengaluru**, **Hyderabad**, and **Kolkata**
- Displays current temperature and weather condition for selected city

###  Current Weather Panel
- Current Temperature (°C)
- Weather Condition (Sunny, Cloudy, etc.)
- Last Updated timestamp

###  7-Day Forecast
- Line chart showing temperature trend from Tuesday to Monday
- Day-wise temperature cards at the top for quick reference

### Weather KPIs
| Metric | Value (Example) |
|--------|----------------|
| Visibility | 6 Km |
| Pressure | 29.88 mm |
| Humidity | 20% |
| Wind Speed | 15.8 Kph |
| UV Index | 8 |
| Precipitation | 0 |

###  Air Quality Index (AQI)
- AQI Donut Chart with status label (**Good / Moderate / Poor**)
- Pollutant breakdown:

| Pollutant | Value |
|-----------|-------|
| CO | 622 |
| NO2 | 15 |
| O3 | 131 |
| PM10 | 28 |
| PM2.5 | 24 |
| SO2 | 19 |

### Sunrise & Sunset
- Sunrise: **06:02 AM**
- Sunset: **06:30 PM**

### 🌧️ Chance of Rain
- Bar chart showing rain probability (%) for each day of the week



## Insights

Here are the key insights derived from the dashboard data for **Hyderabad on 07 April:**

### Temperature Insights
- Current temperature in Hyderabad is **34.3°C** with **Sunny** conditions
- The 7-day forecast shows a **gradual rising trend** — starting at **30.8°C on Tuesday**
  and peaking at **33.7°C on Sunday**, indicating an **approaching heat wave pattern**
- Temperatures dip slightly mid-week (**31.2°C on Thursday**) before climbing again
  towards the weekend
- Among the 3 cities, **Bengaluru is the hottest at 34.4°C**, followed by 
  Hyderabad (34.3°C) and Kolkata (33.2°C)

### Humidity & Comfort Insights
- Humidity is at a **very low 20%**, which means the air is quite dry
- Combined with a temperature of 34.3°C, this creates a **hot and dry climate**
  — uncomfortable for outdoor activities, especially midday
- Low humidity also means **sweat evaporates quickly**, which can lead to 
  **dehydration risks** if not careful

### Wind & Pressure Insights
- Wind speed is **15.8 Kph** — a mild breeze that provides slight relief
  from the heat but is not strong enough for significant cooling
- Atmospheric pressure at **29.88 mm** is within the normal range,
  suggesting **stable weather conditions** with no immediate storm risk

###  Visibility Insights
- Visibility is **6 Km** — moderate visibility
- This could be due to **dust or haze** in the air, which is common during
  hot and dry seasons in Hyderabad
- Not ideal for driving at high speeds or aviation without instruments

###  UV Index Insights
- UV Index is **8**, which falls in the **Very High** category
- This means **unprotected skin can burn in as little as 15–25 minutes**
- Strongly recommended to use **SPF 30+ sunscreen**, wear sunglasses,
  and avoid direct sun exposure between **10 AM – 4 PM**

### Air Quality Insights
- Overall AQI is **28**, which is classified as **"Good"**
- Air is **clean and healthy** — safe for outdoor activities and exercise
- Pollutant-level breakdown:
  - **CO (622)** — Carbon Monoxide is the highest pollutant but still within safe limits
  - **O3 (131)** — Ozone levels are moderate; may cause mild irritation for sensitive groups
  - **PM10 (28)** — Coarse particle matter is low — good for respiratory health
  - **PM2.5 (24)** — Fine particle matter is within acceptable range
  - **NO2 (15)** — Very low nitrogen dioxide — indicates less vehicular/industrial pollution
  - **SO2 (19)** — Very low sulfur dioxide — no industrial burning concerns

###  Chance of Rain Insights
- Rain probability is **100% for all 7 days** — this is a striking pattern
- Despite sunny current conditions and high temperatures, the forecast 
  suggests **significant rainfall is expected throughout the week**
- This could indicate an **approaching monsoon front or a weather system**
  moving into the region
- The combination of **high UV, low humidity today** + **100% rain chance ahead**
  suggests a **sharp weather transition** is expected in the coming days
- Residents should be prepared for **sudden weather changes** —
  carry umbrellas and avoid waterlogging-prone areas

###  Sunrise & Sunset Insights
- Sunrise at **06:02 AM** and Sunset at **06:30 PM** gives approximately
  **12 hours 28 minutes of daylight**
- This is typical for **early April in Hyderabad** as the region approaches summer
- The long daylight hours contribute to **higher UV exposure** and
  **rising daytime temperatures** throughout the week



## Theme & Design

- **Dark mode** background with **orange gradient** accent
- Clean card-based layout for easy readability
- Inspired by a YouTube tutorial for the overall design language



# Tools & Technologies

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Dashboard creation & visualization |
| **WeatherAPI.com** | Live weather data source |
| **Power Query** | Data cleaning & transformation |
| **DAX** | Calculated columns & measures |



##  Steps to Reproduce

1. **Get API Key**
   - Sign up at [WeatherAPI.com](https://www.weatherapi.com/)
   - Generate your free API key

2. **Import Data into Power BI**
   - Open Power BI Desktop
   - Go to `Home → Get Data → Web`
   - Enter the WeatherAPI endpoint URL with your API key

3. **Clean & Transform Data**
   - Open **Power Query Editor**
   - Expand nested JSON columns
   - Separate into 3 tables: `Current`, `Forecast Day`, `Forecast Hours`

4. **Build the Dashboard**
   - Create relationships between tables
   - Build KPI cards, line charts, donut chart, and bar charts
   - Apply the dark theme and orange color scheme

5. **Publish / Share**
   - Save the `.pbix` file
   - Optionally publish to **Power BI Service** for online access
