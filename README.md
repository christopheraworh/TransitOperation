🚍 Transit Operations Analysis – High-Level Summary (README)

This Power BI project provides a comprehensive operational analytics dashboard for a public transit agency. The goal is to help RideCo monitor on-time performance, ridership patterns, and driver reliability through a clean, scalable, and interactive reporting solution.





⭐ Project Overview

![Transit Operation Analysis](./assets/FrontPage Overview.png)
The report transforms raw operational data—rides, shifts, vehicles, passenger types, and locations—into a powerful decision-support tool.
It delivers real-time insights into service delivery, demand behavior, and operational efficiency.

The solution includes:

A hybrid star-schema semantic model optimized for DAX performance

Automated calculations for KPIs like On-Time % and Completion Rate

Interactive drill-downs for drivers, locations, trips, and shifts

Machine Learning–enhanced features for predicting estimated trip durations

📊 Key Metrics & Insights

The dashboard highlights critical KPIs including:

 - Total Rides & Completed Rides

 - On-Time Performance (%)

- Completion & Cancellation Rates

- Average Trip Time

- Average Riders per Hour

- Abandoned Rides


Trend visuals allow RideCo to understand fluctuations in demand and service reliability over time.

Geospatial visuals provide visibility into high-demand pickup/destination zones.

🧠 Data Model

A clean Hybrid Star Schema supports fast, flexible analysis:

Fact Table: Ride-level transactions
Dimensions: Date, Location (Origin & Destination), Passenger Type, Shift, Vehicle

This structure supports:

- Clear slicing/filtering

- Time intelligence

- Role-playing location dimensions

- achine learning integration for trip predictions

🔄 Automation & Scalability

To operationalize the report:

Automated Refresh

- Scheduled refresh in Power BI Service

- Optional incremental refresh for large FactRides

- Fabric Data Factory/Dataflows Gen2 for ingestion

Secure Sharing

- Publish via a Power BI App

- Row-Level Security (RLS) for drivers, supervisors, and regions

Scaling for 100× Data Growth

- Move to a Lakehouse + Delta (Medallion architecture)


- Enable incremental/hybrid refresh for high-volume performance

Use Direct Lake mode for massive datasets

🤖 Machine Learning Integration

A regression model (Python + scikit-learn) was trained using historical trip data to predict travel times.
Predictions are stored in a Delta table and consumed by Power BI, enabling users to select origin/destination points and see estimated trip durations dynamically.

🎯 Outcome

This solution equips transit leadership with:

- Real-time operational visibility

- Driver and fleet performance monitoring

- Insights to improve punctuality, reduce cancellations, and optimize routes

- Predictive capabilities for future planning


Tools | Concepts Utilised
Power BI, DAX, data modeling, Python, machine learning, Fabric analytics engineering and GIT.