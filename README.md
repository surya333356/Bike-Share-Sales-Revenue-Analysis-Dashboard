# Bike-Share-Sales-Revenue-Analysis-Dashboard (SQL + Power BI)
![image](https://github.com/user-attachments/assets/a17c75a0-e5bd-4dc2-b51a-6af116a67a0d)

# Dashboard

![image](https://github.com/user-attachments/assets/b1f6e763-1c6a-4386-bad6-0c3931717747)

# SQL Queries-

COPY bike_rentals 
FROM 'D:/YT_bike_share-main/bike_share_yr_0.csv' 
DELIMITER ',' 
CSV HEADER;



with cte as (select * from bike_share_yr_0
union all
select * from bike_share_yr_1)


select dteday,
season,a.yr,weekday,hr,rider_type,riders,
price,cogs,riders*price as revenue,
riders*price-cogs as profit
from cte a
left join cost_table b
on a.yr=b.yr


End to end Data Analysis Project of PostgreSQL + Power BI included:
🚴‍♂️ Excited to Share My Latest Bike Share Sales & Revenue Analysis Dashboard! 🚀
I recently built a Power BI dashboard powered by PostgreSQL to analyze bike-sharing trends, revenue growth, and profitability over the past two years. 📊
💡 Key Insights:
 ✔ Riders increased by 65% from 2021 to 2022, highlighting growing demand for bike-sharing services.
 ✔ Revenue doubled, rising from ₹4.96M to ₹10.22M, driven by higher ridership and pricing adjustments.
 ✔ Profit surged from ₹3.41M to ₹7.03M, showcasing improved operational efficiency.
 ✔ The average ride price increased from ₹3.99 to ₹4.99, contributing to revenue growth.
🔍 How I Built This Dashboard:
 ✅ PostgreSQL for data extraction & transformation – writing optimized SQL queries to handle large datasets.
 ✅ Power BI for visualization – creating interactive reports to uncover actionable insights.
 ✅ Advanced analytics – trend analysis, revenue forecasting, and profitability tracking.
🚀 Recommendations for Further Growth:
 ✔ Implement dynamic pricing based on demand, weather, and peak hours to maximize revenue.
 ✔ Expand bike stations in high-demand areas to capture more riders.
 ✔ Enhance user experience by improving bike availability, app usability, and customer service.
 ✔ Introduce loyalty programs and promotional offers to boost repeat customers.
This project helped me enhance my expertise in PostgreSQL, Power BI, and data-driven decision-making. Excited to apply these insights to real-world mobility solutions! 🚴‍♂️📊


