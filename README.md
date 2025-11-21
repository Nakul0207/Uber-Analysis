# 🚖 Uber Analytics Dashboard — Power BI

## 📊 Project Overview  
This Power BI dashboard provides data-driven insights into Uber ride performance.  
It focuses on **booking trends, revenue patterns, vehicle performance, cancellations, and customer behavior** to help make business decisions faster and smarter.

---

## 🎯 Objectives
- Analyze booking trends and demand patterns  
- Compare performance of different vehicle types  
- Understand customer behavior and cancellations  
- Identify high-demand locations and peak hours  
- Build insights using DAX measures  

---

## 🧰 Tools & Technologies
| Tool | Purpose |
|------|--------|
| Power BI | Dashboard & Visualizations |
| DAX | Calculations & Measures |
| Excel / CSV | Data Source |
| Power Query | Data Cleaning |

---

## 📂 Dashboard Pages

### 1️⃣ **Overview Page**
- KPIs: Total Bookings, Lost Bookings, Revenue, Total & Avg Distance  
- Monthly booking trend  
- Ratings and cancellations  

**Screenshot:**  
<img width="1819" height="846" alt="Screenshot 2025-11-21 231749" src="https://github.com/user-attachments/assets/42196b96-6ca7-4fd6-8c32-94dd2fb293ca" />


---

### 2️⃣ **Vehicle Analysis**
- Vehicle-wise performance  
- Contribution % (DAX)  
- Customer count by vehicle type  

**Screenshot:**  
<img width="1799" height="850" alt="Screenshot 2025-11-21 231816" src="https://github.com/user-attachments/assets/be763501-5f6d-4f72-a33e-c1be0123c712" />


---

### 3️⃣ **Revenue Insights**
- Revenue by Month & Vehicle Type  
- Top customers  
- Payment method analysis  

**Screenshot:**  
<img width="1809" height="842" alt="Screenshot 2025-11-21 231830" src="https://github.com/user-attachments/assets/b00656e3-7ced-4eb0-ab4e-7dba0fe70e14" />


---

### 4️⃣ **Rider Analysis**
- Rider categories: First Time, Regular, Return  
- Cancellation reasons  
- Customer trend by month  

**Screenshot:**  
<img width="1794" height="866" alt="Screenshot 2025-11-21 231846" src="https://github.com/user-attachments/assets/155131c5-9a6f-4840-b11b-a31cd9cb4968" />


---

### 5️⃣ **Location Analysis**
- Top pickup locations  
- Distance traveled by month  
- Peak booking hours  

**Screenshot:**  
<img width="1807" height="840" alt="Screenshot 2025-11-21 231903" src="https://github.com/user-attachments/assets/f8ea6985-7453-497a-8c01-bc8f8d04e4b8" />


---

## 📌 Key DAX Measures
```DAX
Contribution% =
VAR totalBookings = CALCULATE([Booking_Values], ALL(Uber[Veh_Type]))
RETURN DIVIDE([Booking_Values], totalBookings)

WeekDay =
FORMAT(Uber[Date], "dddd")
```
---

### 🧠 Summary  
This Power BI dashboard converts raw Uber data into meaningful insights, focusing on **customer patterns, vehicle performance, revenue trends, and demand analysis**.  
It helps in making **data-driven business decisions** and highlights opportunities to improve operational efficiency.

---

