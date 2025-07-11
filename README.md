#  Ola Ride Analytics Project

##  Project Overview

Ola Ride Analytics is a data-driven project focused on extracting actionable insights from ride-booking data. The dataset, sourced from Kaggle, represents a simulated set of bookings made on Ola, one of India’s leading ride-hailing platforms. This project showcases the complete data analytics workflow — from data collection and cleaning to cloud-based storage, SQL querying, and data visualization. Using Google Cloud Platform (GCP), I stored and queried the data efficiently with BigQuery, and built dashboards to present key business insights.


##  Project Workflow

### Dummy Data Creation
  - Data generated using an AI model to simulate realistic ride-hailing scenarios.
  - Included entities: bookings, customers, drivers, vehicles, payments.
  - Covered diverse ride statuses, ratings, payment methods, and distances.

### Excel/Google Sheets Staging
  - AI-generated data cleaned and organized in tabular format.
  - Established relationships among entities (e.g., customer ↔ booking, driver ↔ vehicle).

### Cloud Storage & BigQuery Integration
  - Data uploaded to **Google Cloud Storage (GCS)**.
  - Connected and queried using **Google BigQuery** for scalable SQL execution.

### Power BI Visualization
  - Power BI connected directly to BigQuery for real-time data access.
  - Created dashboards to visualize trends, performance metrics, and business insights.

---

## SQL Analysis (Executed in BigQuery)

Here are the business queries tackled using SQL:

1. **Retrieve all successful bookings**
2. **Find the average ride distance per vehicle type**
3. **Total number of cancelled rides by customers**
4. **Top 5 customers by number of rides booked**
5. **Number of driver-cancelled rides (due to personal or car issues)**
6. **Max & min driver ratings for Prime Sedan bookings**
7. **Rides with payment via UPI**
8. **Average customer rating per vehicle type**
9. **Total booking value for successfully completed rides**
10. **List of all incomplete rides with reasons**

### SQL Snapshots:

<img width="1034" height="307" alt=" Find the average customer rating per vehicle type" src="https://github.com/user-attachments/assets/26f42e20-e81a-4290-b41d-d10584325e7a" />
Average customer rating per vehicle type
<br><br>

<img width="1036" height="307" alt=" Find the average ride distance for each vehicle type" src="https://github.com/user-attachments/assets/834406f0-4e17-44f2-b8e7-3114b626f894" />
Average ride distance for each vehicle type
<br><br>
<img width="1054" height="231" alt="List the top 5 customers who booked the highest number of rides" src="https://github.com/user-attachments/assets/4cc31360-71c4-455b-9add-608b62ee56d8" />
Top 5 customers who booked the highest number of rides

---

##  Power BI Dashboards

Visuals created for quick insight and storytelling:


1. **Ride Volume Over Time**  
 

2. **Booking Status Breakdown**  

3. **Top 5 Vehicle Types by Ride Distance**  
 

4. **Average Customer Ratings by Vehicle Type**  


5. **Cancelled Ride Reasons**  


6. **Revenue by Payment Method**  


7. **Top 5 Customers by Total Booking Value**  
 

8. **Ride Distance Distribution Per Day**  


9. **Driver Ratings Distribution**  


10. **Customer vs. Driver Ratings Comparison**  
 

### Power Bi Snapshots:
<img width="1330" height="742" alt="1" src="https://github.com/user-attachments/assets/5ff2bd97-793b-4694-8793-dae30965082e" />
<br><br>
<img width="1305" height="743" alt="2" src="https://github.com/user-attachments/assets/3c9b259d-22ee-4545-9e85-9995e6600238" />





##  Tools & Technologies

- **Google Sheets / Excel** – Initial data staging
- **Cloud Storage (GCS)** – For hosting CSVs before BigQuery load
- **BigQuery (GCP)** – Cloud-based SQL engine
- **Power BI** – Interactive data visualization

---

##  Data model

```text
Customers ─────┐
Drivers   ─────┼──► Bookings ◄─── Vehicles
Payments  ─────┘
