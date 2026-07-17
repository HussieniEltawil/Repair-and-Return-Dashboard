# Repair & Return Dashboard

<p align="center">
  <img src="images/repository-cover.jpg" alt="Repair and Return Dashboard" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Data%20Visualization-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">
  <img src="https://img.shields.io/badge/Power%20Query-Data%20Transformation-217346?style=for-the-badge">
  <img src="https://img.shields.io/badge/DAX-Business%20Logic-B7472A?style=for-the-badge">
  <img src="https://img.shields.io/badge/Supply%20Chain-Analytics-8B1E2D?style=for-the-badge">
</p>

## Project Overview

The **Repair & Return Dashboard** is an end-to-end Power BI solution designed to monitor faulty spare parts throughout the repair and return lifecycle. It gives management a clear view of current position, completion status, bottlenecks, aging, supplier performance, recovery opportunities, stock risk, and cycle time.

The report transforms a complex operational tracker into an interactive decision-support dashboard covering **177 repair and return items**, with dedicated views for open cases, completed cases, overdue targets, supplier concentration, and cumulative forecast versus actual performance.

<p align="center">
  <img src="images/dashboard-preview.gif" alt="Dashboard Preview" width="100%">
</p>

## Business Objectives

- Track the full repair and return process from faulty receipt to warehouse return.
- Identify where open items are currently stopped and which stage creates the largest backlog.
- Monitor overdue and upcoming target dates to support recovery planning.
- Measure supplier workload, geographical footprint, and concentration risk.
- Analyze repair-cycle components and total turnaround time.
- Compare cumulative actual returns against forecast and received faulty items.
- Highlight critical spare parts and stock-shortage exposure.

## Key Dashboard Highlights

| KPI | Value |
|---|---:|
| Total Items | 177 |
| Completed | 70 |
| Open | 107 |
| Received in the Last 30 Days | 26 |
| Upcoming in 30 Days | 8 |
| Oldest Open Case | 407 Days |

## Dashboard Pages

### 1. Current Position & Completion Outlook

Executive view of total items, completed items, open workload, recent receipts, and completion outlook.

![Current Position](images/05-current-position-completion-outlook.png)

### 2. Open Items by Stopping Point

Shows where open cases are currently sitting across repair, RMA confirmation, supplier departure, and SAP PR/PO or delivery stages.

![Stopping Point](images/06-open-items-stopping-point.png)

### 3. Supplier Focus

Ranks suppliers by open items and highlights concentration risk among the leading suppliers.

![Supplier Focus](images/08-supplier-focus.png)

### 4. Aging & Critical Attention

Surfaces the oldest open cases and the items requiring immediate operational follow-up.

![Aging](images/10-aging-critical-attention.png)

### 5. Cumulative S-Curve

Compares cumulative faulty receipts, forecasted returns, and actual returns to warehouse while measuring variance to plan.

![Cumulative S Curve](images/13-cumulative-s-curve.png)

### 6. Monthly Closure Performance

Tracks monthly faulty receipts, arrivals at supplier, and closed or received-back items.

![Monthly Closure](images/14-monthly-closure-performance.png)

### 7. Cycle Time by Step

Breaks the total repair and return cycle into RMA, AWB, warehouse-to-supplier, repair, and warehouse-delivery stages.

![Cycle Time](images/15-cycle-time-by-step.png)

### 8. Monthly Cycle Performance

Displays monthly movement in average cycle days and helps identify months with abnormal delays.

![Monthly Cycle](images/16-monthly-cycle-performance.png)

### 9. Critical Spare Parts & Stock Risk

Compares faulty quantities with stock on hand and identifies critical shortage groups.

![Stock Risk](images/18-critical-spare-parts-stock-risk.png)

## Key Insights

- The report contains **107 open items compared with 70 completed items**, showing that the current backlog remains the primary management priority.
- **Pending Repair** is the largest open stopping point, followed by pending RMA confirmation and pending departure from supplier.
- The oldest open cases exceed one year, indicating the need for targeted escalation and owner-level follow-up.
- Supplier workload is concentrated among a small number of suppliers, creating dependency and recovery risk.
- The total average repair and return cycle is driven mainly by warehouse delivery and repair duration.
- The cumulative S-curve provides a clear comparison between planned returns and actual warehouse receipts.

## Data Preparation & Modeling

The project included:

- Cleaning and standardizing tracker fields using Power Query.
- Correcting data types and handling blank or inconsistent dates.
- Building a dynamic calendar table for monthly analysis.
- Creating relationships between the calendar and process-date fields.
- Developing DAX measures for current status, aging, cumulative totals, forecast variance, cycle time, and recovery metrics.
- Designing interactive navigation and dedicated analytical directories.

## Core DAX Areas

- Total, Open, and Completed Items
- Cumulative Faulty Parts Received
- Cumulative Forecast
- Cumulative Received to Warehouse
- Forecast Variance and Variance Percentage
- RMA, AWB, Repair, Supplier, Warehouse Delivery, and Total Cycle
- Aging Buckets and Oldest Open Age
- Upcoming and Overdue Targets
- Supplier Concentration
- Repairability and Stock Risk Metrics

## Tools & Skills

- **Power BI Desktop**
- **Power Query**
- **DAX**
- **Data Modeling**
- **Operational Analytics**
- **Supply Chain Analytics**
- **KPI Design**
- **Dashboard Design**
- **Performance Monitoring**

## Repository Structure

```text
Repair-and-Return-Dashboard/
├── README.md
├── LICENSE
├── images/
│   ├── 01-main-directory.png
│   ├── 02-project-cover.png
│   ├── ...
│   ├── 43-appendix-4.png
│   ├── dashboard-preview.gif
│   └── repository-cover.jpg
├── docs/
│   └── Repair-and-Return-Dashboard.pdf
└── source/
    └── Repair-and-Return-Dashboard.pbix
```

## Full Report

[View the Dashboard PDF](docs/Repair-and-Return-Dashboard.pdf)

## Author

**Hussieni Eltawil**  
Data Analyst | Power BI Developer | Excel Analyst

- GitHub: [HussieniEltawil](https://github.com/HussieniEltawil)

---

<p align="center"><b>Built with Power BI, Power Query, DAX, and operational business analysis.</b></p>
