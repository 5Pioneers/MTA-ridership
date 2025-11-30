# MTA-ridership
## MTA ridership analysis &amp; visualizations

# Overview
- This project presents an interactive MTA Ridership Dashboard designed to analyze systemwide ridership patterns, on-time performance, peak utilization, payment methods, and station-level trends across multiple transit modes.
- The dashboard supports transportation planners, analysts, and decision-makers in monitoring ridership recovery, service reliability, and demand behavior over time.

# Data Sources
The dashboard uses official datasets from MTA Open Data, including:
1. Subway Hourly Ridership
(Entries by hour, station, and payment method)
2. Daily Ridership & Traffic Data
(Subways, Buses, LIRR, Metro-North, SIR, Access-A-Ride, Bridges & Tunnels)
3. Subway Terminal On-Time Performance (OTP)
(% of trains arriving on time by line, division, and day type)
The dashboard includes year-based filtering (2022–2024) to compare historical patterns and recovery trends.

# Tools
- Power BI – data loading, modeling, transformations, and visualizations
- Tableau – additional visualization and comparative reporting

# Data Preparation

## Data Cleaning
- Split date and time into separate fields
- Corrected Station Complex ID data type (number → text) to resolve format errors
- Added Day Name and Day Type (Weekday vs Weekend) columns

## Data Modeling (Star Schema)
- Created a central Calendar Table for time intelligence
- Linked fact tables:
  Daily Ridership
  Subway Hourly Ridership
  Terminal OTP
- Enabled consistent filtering and cross-dataset analysis

# Key Metrics & Analyses

## Core Ridership KPIs
- Total ridership, transfers, average/max/min daily use

## Time Intelligence
- MTD, YTD, last 7 days, last month, YoY growth

## Peak vs Off-Peak
- Rush-hour demand, off-peak share, peak % contribution

## Payment Methods
- OMNY vs MetroCard usage, adoption trends

## Station-Level Analysis
- Busiest stations, entries, transfers, top-performing locations

## On-Time Performance (OTP)
- Weekday vs weekend reliability
- Performance variations by line (IRT, IND, BMT)
- Correlation between OTP and ridership declines

## Pandemic Recovery
- Recovery % vs 2019 baseline
- Behavior shifts (hybrid work, weekend travel patterns)

# Exploratory Data Analysis (EDA) – Summary
- Residential stations show faster recovery than Manhattan hubs
- Peak hour ridership decreased; mid-day and off-peak rising
- OMNY adoption continuously growing
- Weekend ridership still below weekday levels
- Bus ridership remains behind subway recovery
- OTP variations directly affect demand on certain lines

# Limitations
- Some datasets update at different frequencies
- No demographic segmentation
- External factors (weather, fare policy changes) not included
- OTP reflects terminal arrivals only
- Dashboard focuses on historical analysis; no forecasting models included

# Conclusions
The MTA Ridership Dashboard provides a comprehensive view of transit performance across financial, operational, and behavioral dimensions. It helps identify:
- Recovery strengths and weaknesses
- Peak vs non-peak usage patterns
- High-demand stations and corridors
- Payment method transitions
- Reliability impacts on ridership

## Supports decision-making in:
- Service planning
- Schedule optimization
- Fare policy evaluation
- Infrastructure investment

## Future Enhancements
- Predictive ridership forecasting
- Rider segmentation

Integration of service alerts and weather data

Advanced OTP and reliability analytics
