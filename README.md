# Realtime-SQL-Server-Dashboard-sales-analysis
Live, dynamic sales analytics using Power BI connected to SQL Server.
## Project Overview
A real-time Power BI sales dashboard powered by SQL Server, enabling interactive monitoring of live sales data. The dashboard supports DirectQuery and real-time streaming scenarios, offering near-instant insights into performance.
## Key Technologies & Architecture
- **SQL Server:** Holds sales, customer, and product transaction data.
- **Power BI Desktop & Power BI Service:**
   - **DirectQuery Mode** for live SQL Server queries — enables near-real-time analytics. 
   - **Streaming / Push Datasets** (optional) for live dashboard tiles — supports push and streaming semantic models. 
    Microsoft Learn
   - **Automatic Page Refresh** to keep visuals up to date (especially for DirectQuery sources). 
    Microsoft Fabric Community
- **Power BI Gateway:** Supports live connections to on-prem SQL instances when deployed.
## Features & Dashboard Layout
- **KPI Highlights:** Real-time total sales, average order value, and trending metrics.

- **Live Trend Charts:** Hourly and daily sales visuals using live DirectQuery or streaming data.

- **Segmenting & Drill-down:** Slicers for category, region, sales rep, time period.
  
- **Geospatial Insights:** (Optional) Integrate map visuals to highlight regional activity.
  
- **Real-Time Alerts:** Alerts for thresholds like low stock or sales spikes.
 ## Repository Structure 
 ```bash
 realtime-SQL-Server-Dashboard-sales-analysis/
├── data/
│   └── init_sample_data.sql     # Sample sales table creation and demo data
├── dashboard/
│   └── SalesDashboard.pbix      # Power BI File (DirectQuery/Streaming setup)
├── docs/
│   ├── architecture.png         # System architecture diagram
│   └── user_guide.md            # Instructions for setup and use
├── README.md
└── requirements.txt             # List of dependencies/tools
```
## Getting Started
**1. Clone Repository**

```bash
Copy
Edit
git clone <repo-url>
cd realtime-SQL-Server-Dashboard-sales-analysis/
```
**2. Set Up SQL Server Data**

 - Execute init_sample_data.sql to create sample tables and seed the data.

**3. Open the Power BI Dashboard**

 - Launch SalesDashboard.pbix in Power BI Desktop.

 - Connect to SQL Server using DirectQuery, or configure a Push Dataset via REST or Azure Stream Analytics as needed. 

**4. Configure Refresh Behavior**

 - Enable Automatic Page Refresh (DirectQuery mode) or streaming tiles for live updates. 

**5. Deploy to Power BI Service**

 - Publish the dashboard.

 - Optionally set up a Power BI Gateway (for on-prem data) to maintain live connectivity.
## Real-World Reference
Inspired by the AdventureWorks real-time sales dashboard using DirectQuery mode. 

Also incorporates concepts from frankolanari’s Sales Management Dashboard that connects Power BI with SQL to surface KPIs and performance trends.

## Future Enhancements
- Introduce push streaming datasets to support near-instant dashboard updates.

- Add threshold-triggered notifications or mobile alerts.

- Integrate geospatial visualizations for location-based insights.

- Incorporate predictive analytics using time series modeling for forecasting.
## License & Contributing
- **License: MIT** (or your choice)

- **Contributions:** Pull requests and feedback are welcome! Please fork and submit improvements.
