# DC Slotting & Space Management Portfolio

## Overview

This repository demonstrates my approach to distribution center slotting, space optimization, and inventory flow management from a manager-level operational perspective. The portfolio is designed to mirror real-world DC slotting and flow responsibilities, with a strong emphasis on Excel-driven decision support, KPI management, and WMS-aligned concepts.

All data used is mock or simulated and intended solely to demonstrate analytical methods, operational thinking, and leadership approach. No proprietary systems, layouts, or datasets are included.

---
## Download the Excel Model

The full Excel-based slotting and space management model used in this portfolio is available for download below.

[Download the Excel Slotting & Space Management Model](docs/DC_Slotting_Space_Management_Model.xlsx)

The spreadsheet includes:
- Controlled master data lists
- SKU-level operational inputs
- ABC classification logic
- Pick-face capacity and utilization analysis
- Hazmat slotting controls
- Leadership-ready pivot summaries
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
How to Navigate This Repository

This repository is designed to be reviewed in a logical, top-down flow that mirrors how slotting and space management decisions are made in a real distribution center environment.

Readers should follow this order:

Review the Overview and Purpose sections to understand the business intent and scope.

Walk through the Excel Slotting Model – Visual Walkthrough to see how data flows from raw SKU inputs to leadership-level decisions.

Review the Screenshots section in sequence to understand how each component supports operational decision-making.

Read What I’d Improve With Live WMS Data to see how this model transitions from Excel to SAP or SAP S/4HANA.

Finish with How I’d Operationalize This in 30–60–90 Days to understand execution, ownership, and scale.

This structure is intentional and mirrors how I would onboard stakeholders into a slotting and space optimization initiative.

Note on Screenshots

The screenshots in this repository represent a simulated but WMS-aligned slotting and space management model.

All logic, calculations, and KPIs are intentionally designed to reflect how decisions would be made using live SAP or SAP S/4HANA WMS data, while avoiding the use of proprietary systems, layouts, or datasets.
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
  

All screenshots below are taken directly from the Excel model linked above and represent a simulated but WMS-aligned slotting environment.
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
Slotting and Space Management KPIs

What We Measure, Why It Matters, and How Often We Review It

Effective slotting is not about constant rework. It is about monitoring the right signals at the right cadence. The KPIs below are intentionally selected to balance operational stability, flow efficiency, safety, and scalability, while reducing unnecessary management noise over time.
---
Weekly KPIs – Tactical Control

Audience: Operations Managers, Inventory Control, Floor Leadership
Purpose: Detect and resolve issues early before they impact service, labor, or safety

Percent of SKUs Over Pick-Face Capacity

Why this matters
This metric identifies congestion risk, overflow picking, and excessive replenishment activity. Over-capacity pick faces are a leading indicator of inefficiency and operational friction.

Action taken -
Trigger targeted re-slotting, pick-face expansion, or replenishment frequency adjustments.
---
Percent of A-Items Outside Fast Pick Zones

Why this matters
High-velocity SKUs account for a disproportionate share of labor and travel time. When A-items are not placed in fast or golden zones, avoidable waste is introduced into the picking process.

Action taken -
Prioritize re-slotting A-items into appropriate high-efficiency pick zones.
---
Weekly Replenishment Frequency by SKU

Why this matters
Excessive replenishment indicates poor slot sizing or misalignment between demand and pick-face capacity. This drives additional labor, congestion, and error risk.

Action taken -
Resize pick faces or adjust stocking strategies to stabilize inventory flow.
---
Monthly KPIs – Optimization and Trend Analysis

Audience: Distribution Center Leadership, Continuous Improvement, Planning
Purpose: Validate improvements and prevent regression

Pick-Face Utilization Distribution

Why this matters
This KPI confirms whether pick faces are underutilized, overutilized, or properly sized. It ensures that available cube is aligned with actual demand.

Action taken -
Refine slotting standards, cube assignments, or layout strategies.
---
Congestion Risk by Pick Zone

Why this matters
Zone-level congestion highlights structural flow issues rather than isolated SKU problems. It supports informed decisions related to zone balancing and layout adjustments.

Action taken -
Rebalance zones or adjust labor deployment strategies.
---
Hazmat Slotting Compliance Rate

Why this matters
Hazmat compliance carries zero tolerance. This metric ensures hazardous materials remain in approved, controlled locations and reduces safety and regulatory risk.

Action taken -
Immediate corrective action and escalation if compliance thresholds are breached.
---
Quarterly KPIs – Strategic Alignment

Audience: Senior Leadership, Engineering, Information Technology
Purpose: Ensure slotting strategy supports growth, seasonality, and scalability

Slotting Stability Index

Percent of SKUs requiring re-slotting over the quarter

Why this matters
High slotting churn signals unstable demand modeling or poor slot design. Stability indicates a mature, well-governed slotting strategy.

Action taken -
Reassess velocity thresholds, slotting rules, or replenishment logic.
---
Labor Efficiency Impact from Slotting Changes

Why this matters
This KPI directly links slotting decisions to productivity and cost outcomes. It justifies continued investment in slotting optimization initiatives.

Action taken -
Scale successful slotting strategies and retire low-impact changes.
---
Seasonal Readiness Score

Why this matters
This metric evaluates preparedness for peak seasons, promotions, or assortment changes. It prevents reactive re-slotting during high-volume periods.

Action taken -
Execute pre-peak slotting adjustments and reserve capacity planning.
---
KPI Focus Philosophy

As slotting maturity increases, manual oversight should decrease.

Weekly reviews focus on tactical exceptions only.
Monthly reviews validate trends and optimization efforts.
Quarterly reviews address strategy, automation, and scalability.

The objective is not to review more data, but to review fewer, higher-quality exceptions.
---
Outcome

Slotting and space management evolves from reactive, manual intervention into a continuous, data-driven process that is embedded into daily operations and aligned with leadership decision-making.
## Disclaimer

All examples in this repository are fictional and for demonstration purposes only. They are not based on any specific company’s proprietary data, layouts, systems, or processes.

---

## Author

**Geoffrey Threats**  
MBA -ERP, MS - MIS, MS -Advanced Data Analytics
---
Distribution Center Operations | Slotting & Space Management | Analytics-Driven Leadership

