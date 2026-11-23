# Flight Delay Analysis - Power BI Dashboard

An interactive Power BI dashboard that analyses airline flight data. It covers flight volumes, on-time performance and departure/arrival delays across carriers, origin airports, destinations and months.

## Overview

This project turns raw flight records into a three-page interactive report. Users can track overall performance on KPI cards, find delay patterns by carrier and time period, and explore traffic by origin and destination using slicers and charts.

## Tools Used

- Power BI Desktop
- DAX (custom measures)
- Dark report theme with a custom logo

## Repository Contents

| File | Description |
|------|-------------|
| `flights_dashboard.pbix` | Power BI report with data model, measures and 3 report pages |
| `screenshots/` | Screenshots of each report page (add yours here) |

## Dashboard Pages

### 1. Dashboard Overview (landing page)
High-level snapshot of flight operations.
- KPI cards: Total Flights, On Time Flights, On Time %, Avg Departure Delay, Avg Arrival Delay, Total Scheduled Air Time
- Line chart: Total Flights by Month
- Combo chart: Top 10 Destinations by Month
- KPI visuals: Air Time by Day and Delayed Flights by Month/Hour

### 2. Flight Performance
Focused on delays and punctuality.
- Funnel chart: On Time Flights vs Delayed Flights
- Area chart: Avg Arrival Delay by Carrier
- Column chart: Avg Departure Delay by Year, Month and Day
- Cards: Arrival Delay, Arrival Time, Scheduled Departure Time
- Month slicer

### 3. Flight Data
Traffic breakdown across the network.
- Bar chart: Total Flights by Carrier
- Ribbon chart: Total Flights by Origin
- Area chart: Total Flights by Destination
- Pie chart: Total Flights by Departure Delay
- Origin slicer

Arrow buttons on each page let you navigate between pages.

## Data Fields

| Field | Description |
|-------|-------------|
| `origin` | Departure airport |
| `dest` | Destination airport |
| `carrier` | Airline carrier code |
| `dep_delay` | Departure delay |
| `arr_delay` | Arrival delay |
| `air_time` | Time in the air |
| `sched_dep_time` | Scheduled departure time |
| `sched_arr_time` | Scheduled arrival time |
| `arr_time` | Actual arrival time |
| `time_hour` | Date and hour of the flight |
| `month`, `day`, `hour` | Date and time components |

## DAX Measures

| Measure | Purpose |
|---------|---------|
| `total flights` | Count of all flights |
| `on time flights` | Count of on-time flights |
| `delayed flights` | Count of delayed flights |
| `on time %` | Share of flights that were on time |
| `avg departure delay` | Average departure delay |
| `avg arrival delay` | Average arrival delay |

## Key Features

- Interactive slicers for month and origin airport
- Page navigation buttons
- Time-based analysis by month, day and hour
- Carrier, origin and destination comparisons
- Dark theme with a custom travel logo

## Screenshots

Add screenshots of each page here:

```markdown
![Dashboard Overview](screenshots/overview.png)
![Flight Performance](screenshots/performance.png)
![Flight Data](screenshots/flight-data.png)
```

## How to Use

1. Download `flights_dashboard.pbix`.
2. Open it in **Power BI Desktop** (free to download from Microsoft).
3. Use the page arrows to move between pages.
4. Use the slicers to filter by month or origin airport.

## Data Source

Add the source of your flight dataset here (for example, a public flights dataset or an airline/airport data portal).

## Future Improvements

- Add a carrier comparison page
- Add a delay-cause analysis
- Add a map visual for origin and destination airports
- Publish the report to Power BI Service

## Author

*Akhildas*
