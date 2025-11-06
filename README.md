# ✈️ Indian Airline Passengers Data Dashboard – Power BI Project

## 📌 Project Overview
This Power BI dashboard provides a comprehensive visualization of **Indian Airline Passenger Data**, focusing on insights related to **seat classes, age groups, gender distribution, departure cities, and flight status**.  

The goal is to transform raw passenger data into meaningful business insights, helping airlines understand performance metrics, passenger demographics, and cancellation trends.

---

## 🧰 Tools & Technologies
- **Power BI Desktop** (Data Cleaning, Modelling, Visualization)
- **Excel** (Data Source)
- **DAX** (Custom Measures and KPIs)

---

## 📂 Dataset
The dataset contains passenger-level information with fields such as:
- Full Name  
- Age & Age Group  
- Gender  
- Flight Number  
- Departure & Destination  
- Ticket Price  
- Seat Class  
- Flight Status  

---

## 🧠 Key Measures (DAX)
```DAX
Total Passengers = COUNTROWS(Passengers)

Total Revenue = SUM(Passengers[TicketPrice])

Average Ticket Price = AVERAGE(Passengers[TicketPrice])

Cancellation Rate =
DIVIDE(
    CALCULATE(COUNTROWS(Passengers), 'Passengers'[Status] = "Cancelled"),
    [Total Passengers],


📊 Dashboard Pages
🧩 Page 1: Indian Airline Passengers Data Dashboard

Purpose: Present high-level insights and KPIs

Visuals Included:

KPI Cards — Total Passengers, Revenue, Average Price, Male/Female Count, Cancellation Rate

Donut Chart — Passenger Distribution by Seat Class

Ribbon Chart — Total Revenue by Age Group and Seat Class

Column Chart — Passengers by Departure City and Status

Bar Chart — Passengers by Age Group and Gender

Interactive Filters — Seat Class, Age Group, Gender, Status

🧾 Page 2: Flight-Level View

Purpose: Provide a detailed operational view of each flight

Visuals Included:

Matrix Table showing FlightNumber, SeatClass, TicketPrice, and Status

Conditional Formatting for quick status identification

Aggregated totals for each Seat Class and overall Ticket Price

🎯 Key Insights

31–50 Age Group contributes the highest revenue.

Business Class dominates in both passenger count and ticket revenue.

Delhi, Bangalore, and Mumbai show the highest passenger volume.

Average Ticket Price ≈ ₹846

15% flights were cancelled, providing a key operational improvement area.

🌟 Highlights

Clean and intuitive dashboard layout.

Dynamic interaction through slicers and filters.

Balanced color theme and clear KPI presentation.

Professional storytelling with navigation between overview and detail pages.

🖼️ Dashboard Previews

Page 1: Overview Dashboard


Page 2: Flight-Level View


📤 How to Use

Download the .pbix file from this repository.

Open it using Power BI Desktop.

Explore insights interactively using the slicers and filters.

⭐ Show Some Love

If you found this project useful, please star ⭐ the repo and share your feedback.
Let’s connect and talk data-driven insights!
