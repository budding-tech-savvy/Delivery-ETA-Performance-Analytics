https://datastudio.google.com/reporting/c00de4e5-93d8-452c-9f3c-eb93af7c7809

# 🚚 Delivery ETA Performance Analytics

### Tech Stack

**MySQL | Python | Power BI**

### Project Overview

In e-commerce and logistics, customers expect accurate delivery promises and timely shipment updates. However, measuring delivery performance is not as straightforward as comparing the delivery date against the order date. Different carriers, shipping services, SLAs, and operational exceptions make ETA tracking a complex analytical problem.

To solve this challenge, I developed an end-to-end **Delivery ETA Performance Analytics Framework** that calculates expected delivery dates, measures delivery compliance, identifies operational bottlenecks, and provides actionable insights through an interactive Power BI dashboard.

---

## Business Problem

The logistics team needed a reliable way to answer critical business questions:

* Are shipments being delivered within the promised ETA?
* Which carriers consistently meet delivery commitments?
* How often do operational delays occur?
* What percentage of shipments experience clock-stop events?
* Which zones, customer segments, or shipping methods contribute most to delivery delays?
* Are we meeting organizational targets for customer delivery experience?

Without a standardized ETA measurement framework, performance evaluation across carriers and shipping services was inconsistent and difficult to scale.

---

## Solution Approach

I designed a comprehensive ETA performance framework consisting of three major components:

### 1. ETA Calculation Engine

Mapped shipping options to:

* Carrier services
* SLA business days
* Delivery commitment rules

Using shipment creation dates and SLA definitions, I calculated shipment-level expected delivery dates (ETA).

The framework automatically adjusts for:

* Different shipping methods
* Carrier-specific service commitments
* Business-day based calculations

---

### 2. Compliance & Exception Tracking

Created business rules to classify every shipment into:

#### ✅ On-Time Delivery

Shipment delivered on or before the calculated ETA date.

#### ❌ Late Delivery

Shipment delivered after the promised ETA.

#### ⏸ Clock-Stop Events

Operational exceptions where delivery timelines should not count against carrier performance, such as:

* Customer unavailable
* Address issues
* Weather disruptions
* Delivery reschedule requests

This helped create a fair and accurate measurement system.

---

### 3. Performance Monitoring Dashboard

Built an interactive Power BI dashboard to monitor delivery performance across multiple dimensions.

### Key KPIs

#### ETA Compliance %

Percentage of shipments delivered within promised ETA.

#### Delivered ETA %

Percentage of delivered shipments meeting ETA commitments.

#### Clock-Stop Scan %

Share of shipments impacted by operational exceptions.

#### Carrier Activity %

Carrier-wise shipment contribution and performance.

#### Transit Cycle Time

Average time taken from shipment creation to delivery.

#### Weekly Performance Trends

Tracking delivery performance over time.

---

## Dashboard Features

### Carrier Performance Analysis

Compare delivery efficiency across carriers and identify underperforming partners.

### Zone-Level Insights

Analyze delivery performance across geographical regions.

### Customer-Level Monitoring

Track delivery experience for different customer segments.

### Weekly Trend Analysis

Monitor performance fluctuations and identify recurring operational issues.

### Drill-Down Capability

Move from high-level KPIs to shipment-level details for root cause analysis.

---

## Technical Implementation

### MySQL

* Data extraction
* Shipment tracking data preparation
* Carrier service mapping
* KPI calculation logic
* Data modeling

### Python

* Data cleaning
* Exception handling
* Business-day calculations
* ETA generation logic
* Data transformation and validation

### Power BI

* Interactive dashboards
* KPI scorecards
* Trend analysis
* Carrier comparison reports
* Executive-level performance reporting

---

## Business Impact

The solution enabled stakeholders to:

* Monitor delivery commitments in real time
* Identify carrier-specific performance gaps
* Track operational exception rates
* Improve accountability across logistics partners
* Support organizational targets of:

### 🎯 97% ETA Compliance

### 🎯 95% On-Time Delivery Performance

The framework transformed raw shipment data into actionable operational insights, helping logistics teams make faster and more informed decisions.

---

## Key Learnings

Through this project, I strengthened my skills in:

* Logistics Analytics
* Supply Chain KPI Design
* SLA Performance Measurement
* MySQL Data Modeling
* Python Data Processing
* Power BI Dashboard Development
* Business Problem Solving
* Data-Driven Decision Making

---

## Future Enhancements

* Predictive ETA using Machine Learning
* Delay Risk Prediction Models
* Real-Time Shipment Monitoring
* Automated Alert System for SLA Breaches
* Carrier Performance Forecasting

---

### Final Outcome

This project demonstrates how data analytics can be leveraged to improve delivery reliability, enhance customer experience, and drive operational excellence within logistics and e-commerce operations.
