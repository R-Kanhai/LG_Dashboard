# LG_Dashboard
Interactive Power BI dashboard for ReckDrive Logistics, tracking total orders, on-time delivery rate, CSAT% scores, and average delivery time across hubs, drivers, and vehicles. Features MoM KPI trends, hub capacity charts, driver scatter plots, plus fleet breakdown insights, all filterable by year and month with cross-highlighting interactivity.
# 🚚 ReckDrive Logistics Dashboard

An interactive **Power BI** dashboard built to give logistics operations teams real-time visibility into order performance, hub efficiency, driver productivity, and fleet health — all in one place.

![Power BI](https://github.com/R-Kanhai/LG_Dashboard/blob/main/Logistic%20Dashboard.png)


---

## 📌 Overview

SwiftRoute Logistics operates a multi-hub delivery network and needed a single source of truth to monitor daily operations — order volume, delivery performance, hub throughput, driver behavior, and vehicle reliability. This project translates that business need into a two-dashboard Power BI solution with four focused pages, each designed around a specific business question and audience.

**Live demo:** *[add your Publish-to-Web link here]*
**Screenshots:** *[add dashboard screenshots / GIF here]*

---

## 🗂️ Dashboard Structure

### Dashboard 1 — Overview
The executive summary page. Four headline KPIs, each with current month, previous month, and MoM % change:

| KPI | What it tracks 
| **Total Orders** | Order volume for the selected year/month |
| **On-Time Delivery Rate (%)** | Share of orders delivered on time |
| **Customer Satisfaction (CSAT %)** | Overall customer satisfaction score |
| **Average Delivery Time (Hrs)** | Average time to complete a delivery |

Supporting visuals cover Hub, Driver, and Vehicle snapshots — total hub/driver/vehicle counts, orders vs. hub capacity, hub performance ranking, driver experience vs. rating, active vehicle share, and orders by vehicle model.

### Dashboard 2 — Deep Dive Pages

**Hubs Overview**
- Total number of hubs (KPI card)
- Orders processed vs. hub capacity (clustered column chart)
- Hub performance ranking (ranked bar chart)
- Hub order processing time by day (matrix chart)

**Drivers Overview**
- Number of active drivers (KPI card)
- Experience vs. rating (scatter plot)
- Drivers with the most delays (bar chart)
- Individual driver profile summary — hire date, years of experience, star rating, monthly deliveries (KPI card)
- Monthly order trend (line chart)

**Vehicles Overview**
- Number of vehicles / active vehicles (KPI card + donut chart)
- Total orders by vehicle model (bar chart)
- Vehicle age vs. breakdown frequency (scatter chart)
- Breakdowns by vehicle code and model (bar charts)
- Orders by vehicle type (donut chart)

---

## ✨ Key Features

- **Dynamic Year/Month filtering** across every page via slicers
- **Month-over-Month (MoM) comparisons** built with DAX time-intelligence measures
- **Cross-highlighting** — clicking any visual filters related visuals on the same page
- **Drill-through / tooltip pages** for contextual detail without cluttering the main view
- **Ranked and scatter visuals** to surface top/bottom performers and outliers at a glance

---

## 🧱 Data Model

Built on a star-schema structure:
- **Fact tables:** Orders, Hub Activity, Driver Deliveries, Vehicle Breakdowns
- **Dimension tables:** Hubs, Drivers, Vehicles, Date
- A shared **Date dimension** drives all time-intelligence DAX measures (previous month, MoM % growth/decline)

---

## 🛠️ Tech Stack

- **Power BI Desktop** — data modeling, DAX, report design
- **Power Query** — data cleaning and transformation
- **DAX** — KPI and time-intelligence calculations

---

## 🚀 How to Explore

1. Open the `.pbix` file in Power BI Desktop, 
2. View the interactive version via the Publish-to-Web link above (no login required)
3. Use the **Year/Month slicers** at the top of each page to filter the entire report
4. Click any chart, bar, or point to cross-filter the rest of the page
5. Hover over visuals for tooltip detail; use the page tabs to navigate between Overview, Hubs, Drivers, and Vehicles

---

## 📁 Repository Contents

```
├── ReckDrive_Logistics_Dashboard.pbix   # Power BI report file
├── Business_Requirements.docx            # Source requirements document
├── /screenshots                          # Dashboard preview images
└── README.md
```

---

## 📬 Contact

Built by Rohan Kanhai as part of a Power BI portfolio project.
https://www.linkedin.com/in/rkanhai/ · rohankanhai55@gmail.com

*Note: This project uses sample/anonymized data for demonstration purposes only.*
