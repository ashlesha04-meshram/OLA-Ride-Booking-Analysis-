# OLA-Ride-Booking-Analysis-
 End-to-end OLA ride booking analysis using SQL, Excel and Power BI.
 
Project Objective:

Analysed 20,000+ OLA ride booking records using SQL and Power BI to understand ride performance, customer behaviour, cancellations, and revenue.

Process:

Collected and understood the 20,000-row dataset.
Checked missing values, duplicates, and data consistency.
Used SQL queries to analyse bookings, cancellations, customer ratings, vehicle types, and revenue.
Used Power BI to create interactive dashboards with charts, KPIs, and filters.
Analysed the results to identify business trends and insights.

Tools Used: 

SQL, Power BI, Excel.

SQL Analysis Performed:

Using SQL, I performed the following basic to advanced analyses on the OLA ride booking dataset:

1. Retrieve all successful bookings:
SELECT * FROM bookings WHERE Booking_Status = 'Success';
2. Find the average ride distance for each vehicle type:
SELECT Vehicle_Type, AVG(Ride_Distance) as avg_distance FROM bookings GROUP BY
Vehicle_Type;
3. Get the total number of cancelled rides by customers:
SELECT COUNT(*) FROM bookings WHERE Booking_Status = 'cancelled by Customer';
4. List the top 5 customers who booked the highest number of rides:
SELECT Customer_ID, COUNT(Booking_ID) as total_rides FROM bookings GROUP BY
Customer_ID ORDER BY total_rides DESC LIMIT 5;
5. Get the number of rides cancelled by drivers due to personal and car-related issues:
SELECT COUNT(*) FROM bookings WHERE cancelled_Rides_by_Driver = 'Personal & Car
related issue';

Key Outcomes:
Identified successful and cancelled booking patterns.
Analysed revenue by payment method.
Compared vehicle performance and ride distances.
Evaluated customer and driver ratings.
Identified top customers by booking value.


Conclusion:
This project helped me develop practical skills in SQL querying, data analysis, Power BI dashboard development, and business insight generation.Key Outcomes:






