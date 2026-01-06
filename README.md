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

## Execution Framework

- 📘 [30-60-90 Day Slotting & Space Management Execution Plan](docs/30-60-90-slotting-execution-plan.md)

## Excel Slotting Model – Visual Walkthrough

### 1. Master Data & Controlled Lists
Centralized reference lists enforce standardized Category, Handling Type, and Hazmat values across the model to prevent inconsistent slotting logic.
![Legend Controlled Lists](screenshots/01-legend-controlled-lists.png)

### 2. Raw SKU Data Structure
SKU-level operational inputs including weekly picks, cube, weight, current location, and pick zone used as the foundation for all downstream analysis.
![Data Raw Table](screenshots/02-data-raw-table.png)

### 3. Data Validation Controls
Dropdown controls restrict user input to approved values, reducing data quality issues and supporting scalable operational use.
![Data Validation Dropdowns](screenshots/03-data-validation-dropdowns.png)

### 4. VLOOKUP Master Data Mapping
Exact-match VLOOKUP logic dynamically populates SKU attributes to simulate WMS-aligned master data relationships.
![VLOOKUP Formula Visible](screenshots/04-vlookup-formula-visible.png)

### 5. Pick Zone Velocity Analysis
Pivot table summarizes weekly pick volume by pick zone to identify high-traffic areas and potential congestion risk.
![Pivot Picks by Zone](screenshots/05-pivot-picks-by-zone.png)

### 6. Interactive Filtering
Interactive filters allow analysis by Category, Handling Type, and Hazmat status to support cross-functional decision reviews.
![Pivot Filters](screenshots/06-pivot-filters.png)

### 7. % of Volume Visualization
Conditional formatting highlights velocity concentration to support ABC classification and zone rebalancing decisions.
![Percent Volume Heatmap](screenshots/07-percent-volume-heatmap.png)

### 8. ABC Classification & Velocity Analysis
ABC logic ranks SKUs by cumulative pick volume to guide slotting priority and pick-face allocation.
![ABC Classification](screenshots/08-abc-classification.png)

### 9. Slotting & Hazmat Decision Logic
Rule-based logic assigns slotting zones while overriding standard placement for Hazmat SKUs to enforce safety controls.
![Slotting Hazmat Logic](screenshots/09-slotting-hazmat-logic.png)

### 10. Pick-Face Utilization & Congestion Risk
Pick-face cube utilization identifies over-capacity SKUs and flags congestion risk requiring re-slotting or face expansion.
![Pick Face Utilization](screenshots/10-pick-face-utilization.png)

### 11. Leadership Pivot Summary
Executive-level summary consolidates velocity, congestion, and Hazmat exposure metrics for leadership review.
![Pivot Summary Leadership](screenshots/11-pivot-summary-leadership.png)

# What I’d Improve With Live WMS Data (SAP / SAP S/4HANA)
This Excel-based model is intentionally designed to mirror how slotting and space management decisions are made in a live WMS environment. With direct access to SAP or SAP S/4HANA WMS data, the following enhancements would be implemented to operationalize and automate decision-making.

## 1. Real-Time Velocity & Demand Signals

Replace static weekly picks with rolling demand windows (7 / 14 / 28 days) sourced directly from SAP:

Outbound deliveries

Pick confirmation data

Identify short-term velocity spikes to proactively:

Adjust pick-face sizing

Reassign pick zones before congestion occurs

## 2. Pick-Face Capacity & Replenishment Triggers

Leverage SAP bin master data (bin cube, max quantity, UOM) to calculate true bin saturation

Convert the “Over Capacity” flag from a static indicator into:

Automated replenishment triggers

Re-slotting recommendations

## 3. Labor & Travel Optimization

Combine pick frequency with:

Travel path data

Task interleaving logic

Identify congestion hot spots within pick modules

Re-slot high-velocity SKUs closer to:

Induction points

Golden zones

High-efficiency pick paths

Reduce picker travel time, fatigue, and congestion-related delays

## 4. Safety & Hazmat Enforcement

Enforce Hazmat slotting rules using SAP:

Material master attributes

Dangerous goods indicators

Automatically prevent Hazmat SKUs from being slotted into:

High-traffic zones

Ergonomically unsafe locations

## 5. Exception-Based Management

Shift leadership focus from reviewing all SKUs to reviewing only exceptions, such as:

Over-capacity pick faces

Hazmat SKUs in non-compliant zones

A-items outside fast pick zones

These exceptions would be surfaced through dashboards, not spreadsheets.

Outcome: Slotting decisions move from reactive, manual reviews to proactive, rules-driven execution embedded directly within WMS workflows.

## How I’d Operationalize This in 30–60–90 Days


30–60–90 Day Slotting & Space Optimization Plan

This phased approach focuses on quick wins, operational alignment, and sustainable improvement while minimizing disruption to daily DC operations.

## First 30 Days — Baseline & Stabilization

Primary Focus: Visibility, trust in data, and safety

Validate current slotting logic, bin standards, and pick-zone definitions within SAP

Establish baseline KPIs:

% of SKUs over pick-face capacity

% of A-items outside fast pick zones

Hazmat slotting compliance

Identify the top 10–20 high-impact SKUs driving:

Congestion

Excessive replenishment

Align with Operations, Safety, and IT on slotting rules and constraints

Deliverables

Slotting baseline report

Initial congestion and safety risk list

Agreed-upon slotting standards

## Days 31–60 — Optimization & Execution

Primary Focus: Reducing congestion and improving flow

Re-slot A-items into fast pick zones using verified velocity data

Expand or split pick faces for chronic over-capacity SKUs

Implement Hazmat-specific reserve or controlled zones

Introduce a weekly slotting review cadence driven by exceptions, not full SKU lists

Deliverables

Measurable reduction in over-capacity SKUs

Updated slotting playbook

Weekly exception dashboard

## Days 61–90 — Automation & Sustainability

Primary Focus: Scale and automation

Automate:

Velocity ranking

Slotting exception reporting
using SAP extracts or reporting tools

Integrate slotting KPIs into standard DC performance reviews

Partner with IT to embed slotting rules into SAP task logic where feasible

Prepare seasonal and peak-volume slotting strategies

Deliverables

Automated slotting exception reports

Leadership-ready KPI dashboard

Peak readiness slotting plan

Outcome: Slotting and space management becomes a continuous, data-driven process instead of a periodic cleanup activity.

---

## Disclaimer

All examples in this repository are fictional and for demonstration purposes only. They are not based on any specific company’s proprietary data, layouts, systems, or processes.

---

## Author

**Geoffrey Threats**  
MBA -ERP, MS - MIS, MS -Advanced Data Analytics
---
Distribution Center Operations | Slotting & Space Management | Analytics-Driven Leadership

