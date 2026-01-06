# DC Slotting & Space Management Portfolio

## Overview

This repository demonstrates my approach to distribution center slotting, space optimization, and inventory flow management from a manager-level operational perspective. The portfolio is designed to mirror real-world DC slotting and flow responsibilities, with a strong emphasis on Excel-driven decision support, KPI management, and WMS-aligned concepts.

All data used is mock or simulated and intended solely to demonstrate analytical methods, operational thinking, and leadership approach. No proprietary systems, layouts, or datasets are included.

---

## Purpose of This Portfolio

This portfolio was created to showcase how I would approach a **Manager, Distribution Center – Slotting & Space Management** role, including:

- SKU velocity analysis and ABC classification  
- Slotting optimization and flow improvement  
- Bin saturation and cube utilization management  
- Replenishment logic and pick-face design  
- Safety and ergonomic slotting principles  
- Seasonal and temporary inventory planning  
- KPI-driven operational reviews  
- Structured 30-60-90 day execution planning  

The focus is on practical execution, measurable impact, and cross-functional alignment with Operations, IT, Safety, and Inventory Planning teams.

---
## Execution Framework

- 📘 [30-60-90 Day Slotting & Space Management Execution Plan](docs/30-60-90-slotting-execution-plan.md)


## Tools & Skills Demonstrated

### Excel Proficiency

This portfolio intentionally emphasizes Excel as a decision-support tool, including:

- Pivot Tables (SKU velocity, ABC analysis, KPI summaries)  
- Formulas (cube utilization, bin saturation %, capacity thresholds)  
- Lookups (VLOOKUP / XLOOKUP for SKU and location attributes)  
- Filters to isolate high-impact SKUs  
- Conditional formatting for risk and congestion flagging  

### Operational & Systems Thinking

- Velocity-based slotting strategy  
- WMS-aligned concepts (locations, bins, pick faces, replenishment triggers)  
- Flow optimization and congestion reduction  
- Capacity planning for seasonal and peak demand  
- KPI definition and review cadence  

VLOOKUP Usage
SKU attributes are also populated using VLOOKUP with exact match against a master reference table to demonstrate traditional Excel lookup proficiency.

## Excel Slotting Model – Visual Walkthrough

### 1. Master Data & Controlled Lists
This tab defines controlled values used across the model to enforce data discipline.

![LEGEND](screenshots/01_legend_controlled_lists.png)

---

### 2. Raw SKU Data Structure
SKU-level operational inputs including picks, cube, weight, and pick zone.

![Data_Raw](screenshots/02_data_raw_table.png)

---

### 3. Data Validation Controls
Dropdowns enforce standardized Category, Handling Type, and Hazmat flags.

![Dropdowns](screenshots/03_data_validation_dropdowns.png)

---

### 4. VLOOKUP Master Data Mapping
SKU attributes dynamically pulled using VLOOKUP.

![VLOOKUP](screenshots/04_vlookup_formula_visible.png)

---

### 5. Pick Zone Velocity Analysis
Pivot table summarizing weekly pick volume by pick zone.

![Pivot – Weekly Picks by Pick Zone](screenshots/05_pivot_pick_zone_summary.png)

---

### 6. Interactive Filtering
Analysis dynamically updates based on Category, Handling, and Hazmat filters.

![Filters – Category, Handling, Hazmat](screenshots/06_pivot_filters_in_use.png)

---

### 7. % of Volume Visualization
Conditional formatting highlights velocity concentration.

![Heatmap – % of Volume by Zone](screenshots/07_percent_of_volume_heatmap.png)

## Repository Structure
dc-slotting-space-management-portfolio/

### 01_strategy/
### 02_velocity/
### 03_optimization/
### 04_capacity/
### 05_replenishment/
### 06_safety/
### 07_seasonal/
### 08_kpis/
### 09_leadership/
── README.md


---

## Disclaimer

All examples in this repository are fictional and for demonstration purposes only. They are not based on any specific company’s proprietary data, layouts, systems, or processes.

---

## Author

**Geoffrey Threats**  
MBA -ERP, MS - MIS, MS -Advanced Data Analytics
---
Distribution Center Operations | Slotting & Space Management | Analytics-Driven Leadership

