# Hotel Booking Anlysis
This project provides insights into hotel booking data — including occupancy trends, cancellations, revenue analysis, and customer behavior pattern.




## 🎯  Key Objectives

- Understand booking patterns based on room type, meal plan, and customer segment.
- Evaluate Average Daily Rate (ADR), revenue trends, and occupancy performance.
- Identify key factors influencing booking cancellations.
- Analyze source and agent performance for better channel management.



## 🔹 Key Features
- Room Type & Meal Plan Analysis  
- Booking Source & Cancellation Rate Visualization  
- ADR (Average Daily Rate) and Revenue Insights  
- Channel & Agent Performance Tracking
  

## 📊 Dataset Information
- Columns: Hotel type, Arrival date, Country, Market segment, Agent, Room type, Meal, ADR, Booking status, etc.
- Source: Kaggle Hotel Booking Dataset or internal property management data.
- Data Cleaning: Missing value handling, outlier detection, and feature formatting.


## 📊 Key Performance Indicators (KPIs)
- KPI Description	DAX / Calculation Idea
- Total Bookings	Count of all bookings	COUNTROWS(Bookings)
- Cancellation Rate	% of canceled bookings	(SUM(is_canceled)/COUNTROWS(Bookings))*100
- Average Daily Rate (ADR)	Average revenue per room per night	AVERAGE(adr)
- Revenue Lost due to Cancellations	Potential revenue from canceled bookings	SUMX(FILTER(Bookings, is_canceled=1), adr)
- Total Guests	Total adults + children + babies	SUM(adults)+SUM(children)+SUM(babies)
- Average Lead Time	Avg days before arrival	AVERAGE(lead_time)

## 💡 Insights

- Higher cancellation rates observed in Online Travel Agent (OTA) bookings.
- City Hotels show higher occupancy but lower ADR compared to Resort Hotels.
- Most guests prefer BB (Bed & Breakfast) meal plans.
- Revenue is highest during summer months, indicating strong seasonal demand.
- Longer lead times correspond to higher booking success rates.


## 📈 Visualizations in Power BI
Visualization	Purpose
-  Bar Chart – Cancellation by Market Segment	Identify which segments have high cancellations
-  Line Chart – ADR by Month	Track room rate trends through the year
-  Gauge Chart – Avg Lead Time Performance	Compare booking lead times against benchmarks
-  Donut Chart – Meal Plan Popularity	Identify top preferred meal plans
- Table / KPI Cards	Display overall performance summary (bookings, cancellations, ADR, guests)
