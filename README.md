# 🏨 Hospitality Insights Dashboard – Data-Driven Decisions for OYO Bookings

Welcome to the **Hospitality Insights Dashboard** – a dynamic and interactive Power BI report designed to unlock valuable business insights from OYO’s hotel booking data. This project simulates a real-world data scenario where hotel chains analyze their performance across cities, room types, and time periods to make smarter, faster, and more informed decisions.

---

## 🌟 About the Project

In the competitive hospitality sector, data can be a game-changer. This dashboard acts as a **decision-support tool** for hotel managers and business teams, helping them track KPIs like occupancy rates, revenue, customer preferences, and booking trends — all in one place.

This project is ideal for:
- Data Analysts/Data Enthusiasts exploring BI reporting
- Hospitality domain stakeholders
- Recruiters reviewing BI project portfolios

---

## 🔍 Project Objectives

The main goals of this project were:

✅ Build a **professional-grade Power BI dashboard** using real-world-like structured data  
✅ Enable stakeholders to **explore bookings and performance** across hotels and room categories  
✅ Apply **data modeling best practices** (Star Schema) for clean, scalable, and efficient analysis  
✅ Demonstrate storytelling with data through clean, actionable visualizations

---

## 🧩 Data Model & Schema Design

This project follows a **Star Schema**, separating facts from dimensions for optimal analytical performance.

### 🗂️ Tables Used:

| Table Name                  | Type        | Description |
|----------------------------|-------------|-------------|
| `fact_aggregated_bookings` | Fact Table  | Contains transactional booking data like occupancy, revenue, and booking dates |
| `dim_hotels`               | Dimension   | Metadata about each hotel such as name, city, state, hotel group |
| `dim_rooms`                | Dimension   | Contains room type, capacity, rate type, and pricing |
| `dim_date`                 | Dimension   | Full calendar table supporting time-series analysis (day, month, quarter, year) |

### 🔗 Key Relationships:
- `BookingDate` links `fact_aggregated_bookings` to `dim_date`
- `HotelID` links bookings to `dim_hotels`
- `RoomID` links bookings to `dim_rooms`

These relationships allow **intuitive slicing and dicing** of data across multiple business views.

---

## 📊 Dashboard Features & Highlights

### 👁️ What Can You Explore?

- 📅 **Time-Based Trends** – Monthly, quarterly, or year-wise performance of hotel bookings and revenue
- 🏨 **Top Performing Hotels** – By occupancy, revenue, or customer interest
- 🛏️ **Room-Level Analysis** – Breakdown by room type, occupancy rate, and price range
- 📍 **Location-Based Filtering** – City-wise hotel performance comparison
- 🔍 **Interactive Slicers** – Filter the entire report by multiple fields (hotel group, state, city, etc.)

> 🎯 Every visual is designed to **help business teams act** – whether it's adjusting pricing, managing inventory, or identifying low-performing properties.

---

## 🛠️ Tools & Technologies Used

| Tool/Tech     | Purpose |
|---------------|---------|
| **Power BI**  | Dashboard creation, DAX-based metrics, user-friendly visuals |
| **CSV/Excel** | Data extraction, transformation, and cleaning |
| **Star Schema Design** | Clean data model for performance & maintainability |
| **DAX**       | Custom metrics (occupancy %, YoY growth, etc.)

---

## 📁 Project Structure

```
📦 hospitality-insights-dashboard/
 ┣ 📊 hospitality_oyo.pbix               → Main Power BI dashboard file
 ┣ 📂 data/
 ┃ ┣ 📄 dim_date.csv                    → Calendar table
 ┃ ┣ 📄 dim_hotels.csv                  → Hotels metadata
 ┃ ┣ 📄 dim_rooms.csv                   → Room-related data
 ┃ ┗ 📄 fact_aggregated_bookings.csv    → Booking transactions
 ┣ 📄 README.md                         → Project documentation
 ┗ 📂 screenshots/                      → (Add dashboard images here)
```

---

## 🚀 How to Run This Project

To explore or customize this dashboard on your own system:

1. Download or clone the repository  
2. Open `hospitality_oyo.pbix` with **Power BI Desktop**  
3. Use slicers and filters to explore metrics and visuals  
4. (Optional) Modify the dataset to connect with a SQL Server or your own source

---

## 💼 Real-World Application

This dashboard mimics a real use case where hotel management can:
- Optimize room pricing based on demand trends
- Identify high-performing and under-performing properties
- Plan marketing campaigns for off-peak seasons
- Track occupancy rates and customer behavior across states

---

## 👤 About the Creator

**Vikas Kumar**  
🎓 Data Analyst | BI Enthusiast | Lifelong Learner  
📫 Reach out via [LinkedIn] www.linkedin.com/in/vikas-ku  
🌐 Portfolio: 

---

## 📄 License

This project is for educational and portfolio purposes only. The data has been anonymized and is used strictly for non-commercial analysis demonstrations.

---

> ✨ *Thank you for checking out this project! I hope it gives you valuable ideas for building impactful dashboards.*  
Feel free to ⭐️ the repo or drop a message if you found this helpful.

