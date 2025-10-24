# Sales-Forecasting-and-BI-Dashboard
This project is a complete, end-to-end business intelligence solution that performs sales forecasting for the Rossmann retail chain.
It follows a full data pipeline:
Extract: Raw CSV data is loaded into a relational database.
Transform: Data is cleaned, processed, and modeled using Python (SARIMAX) to generate a 52-week sales forecast.
Load: The historical data and new forecast are stored in a PostgreSQL database.
Visualize: A multi-page Power BI dashboard connects directly to the database for interactive analysis and insights.

Final Dashboard

Here are the three main pages of the final interactive dashboard.
Page 1: Forecast Overview
Provides a high-level summary of historical performance and future projections.
Page 2: Performance Drivers
Analyzes the "why" behind sales numbers, focusing on promotions, competition, and holiday impacts.
Page 3: Customer Behavior
Dives deep into weekly shopping patterns and the relationship between customers and revenue.

Key Business Insights

This dashboard uncovers several quantifiable insights:
Promotions are Highly Effective: Sales on promotional days (Promo = 1) are, on average, nearly double the sales of non-promotional days.
Weekly Sales Cycle: Sales and customer traffic peak on Monday and steadily decline throughout the week, hitting their lowest point on Sunday (when most stores are closed).
Dominant Store Types: Storetype 'a' and Storetype 'c' are the clear market leaders, accounting for over 98% of all sales. Storetype 'b' is a negligible contributor (1.21%).
Forecasted Rebound: After a sales decline in 2015, the SARIMAX model forecasts a strong sales rebound in 2016, projecting an increase from 1.0B to 1.8B.
Customer vs. Sales: There is a direct, positive correlation between the number of customers and total sales, confirming that driving foot traffic is a successful strategy.

Holiday Impact:
State Holidays (a, b, c): These are not shopping days. The data confirms most stores are closed, leading to near-zero sales.
School Holidays (1): These are key shopping days. Sales on weekdays during school holidays are significantly higher than on normal weekdays, indicating that families are a key customer segment.
