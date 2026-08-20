# Weather Insights Dashboard

**A Power BI dashboard for exploring historical weather patterns and trends**

An interactive Power BI dashboard that analyzes historical weather data — temperature, humidity, pressure, visibility, and wind — to uncover seasonal patterns, yearly trends, and relationships between weather variables.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dashboard Components](#dashboard-components)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Key Insights](#key-insights)
- [Objective](#objective)

---

## Overview

This project presents a single-page, multi-visual Power BI dashboard titled **"Weather Insights"** (subtitled "Breezy – First Summary"). It consolidates historical weather records into a set of interactive charts, tables, and KPI cards, allowing users to explore how temperature, humidity, pressure, wind, and visibility behave across months and years.

## Features

- Interactive Power BI report with cross-filtering visuals
- Daily weather summary breakdown (e.g. Mostly Cloudy, Partly Cloudy, Foggy, Overcast)
- Correlation view between pressure and humidity
- Seasonal temperature trend by month
- Year-wise and month-wise temperature table with totals
- KPI cards summarizing visibility, temperature, wind speed, and day count
- Gauge visualization for total visibility
- Wind bearing vs. wind speed distribution
- Year-wise wind speed breakdown (pie chart)

## Dashboard Components

| Visual | Description |
|---|---|
| **Count of Summary vs Daily Summary** | Bar chart showing frequency of each daily weather condition (e.g. Mostly Cloudy, Foggy, Overcast) |
| **Pressure vs Humidity** | Area chart showing how atmospheric pressure varies with humidity |
| **Sum of Temperature (C) by Month** | Line chart showing seasonal temperature trend, peaking mid-year |
| **Year / Month / Sum of Temperature (table)** | Tabular breakdown of total temperature by year (December data shown), with grand total |
| **Total Visibility, Temperature, Wind Speed & Day Count** | KPI summary cards showing aggregated metrics |
| **Sum of Visibility (gauge)** | Gauge chart showing total visibility (998.03K) |
| **Wind Bearing vs Wind Speed** | Line/area chart showing wind speed distribution across wind bearing values |
| **Wind Speed vs Year (pie chart)** | Proportional breakdown of wind speed by year (2006–2016) |

## Tech Stack

| Category | Tools |
|---|---|
| Visualization & BI | Microsoft Power BI |
| Data Modeling | Power BI (Power Query / DAX) |
| Source Data | Historical weather dataset (daily summary, temperature, humidity, pressure, visibility, wind) |

## Project Structure

```
Weather-Insights-Dashboard/
├── Weather_Insights.pbix     # Power BI dashboard file
├── data/                     # Source weather dataset (CSV/Excel)
└── README.md
```

## Usage

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
2. Clone or download this repository
3. Open `Weather_Insights.pbix` in Power BI Desktop
4. Use the slicers and cross-filtering visuals to explore the data
5. (Optional) Refresh the data source with updated weather records

## Key Insights

- Temperature follows a clear seasonal curve, rising from January and peaking around July–August before declining toward December
- Daily weather conditions are dominated by a small set of recurring summaries (e.g. "Mostly Cloudy"), which appear far more frequently than others
- Humidity shows a strong relationship with atmospheric pressure, with pressure rising sharply at higher humidity levels
- December temperature totals vary considerably year over year (2006–2016), including several years with negative aggregate values
- Wind speed distribution varies notably by year, with certain years contributing disproportionately to total wind speed

## Objective

To transform raw historical weather data into an interactive, easy-to-read dashboard that helps users identify seasonal patterns, yearly trends, and relationships between key weather variables for analysis and decision-making.
