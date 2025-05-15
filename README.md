# 🚴‍♂️ Cyclistic Bike-Share Analysis – Capstone Project

**Author:** Ahmed Salim  
**Level:** Beginner – Google Data Analytics Certificate Project  
**Tools Used:** R, RStudio (Tidyverse, Lubridate, HMS, Data.table), Excel, Power BI  
**GitHub Repo:** [Cyclistic-Bike-Share-Analysis](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis)

---

## 📌 Project Overview
This project is part of the final capstone for the Google Data Analytics Professional Certificate. The goal is to help **Cyclistic**, a fictional bike-share company in Chicago, analyze how **casual riders** and **annual members** use their bikes differently—ultimately helping the marketing team develop a strategy to convert more casual users into members.

---

## 🎯 Business Task
**Main question:**  
How do casual riders and annual members use Cyclistic bikes differently?

By identifying usage patterns over a 12-month period, Cyclistic can build targeted marketing strategies to boost membership subscriptions.

---

## 📂 Dataset
- **Source:** [Divvy Bikes – System Data](https://divvybikes.com/system-data)
- **Provider:** Motivate International Inc.
- **Timeframe:** April 2024 to March 2025
- **Files:** 12 individual `.csv` files
- **Volume:** 5M+ ride records

---

## 🛠️ Tools & Skills Used
- **R**: Data cleaning, transformation, and feature engineering
- **Tidyverse**: Wrangling with `dplyr`, `ggplot2`, `tidyr`
- **Lubridate**: Date and time parsing
- **HMS**: Time classification
- **Data.table**: Exporting data
- **Excel**: Quick reviews & exploration
- **Power BI**: Dashboard development & data visualization
- **RStudio**: R scripting environment

---

## 🧼 Data Cleaning Process (R)
- Merged all 12 monthly `.csv` files
- Filtered out nulls, duplicates, and negative ride durations
- Engineered new features: `ride_length`, `day_of_week`, `season`, `hour`, `time_of_day`
- Removed unused fields like GPS and station IDs
- Exported the cleaned dataset to `.csv` for Power BI visualization

📄 R Script: [`cyclistic_analysis.R`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/cyclistic_analysis.R)

---

## 📊 Dashboard & Visualizations
Built an interactive dashboard in Power BI featuring:
- Total rides and ride duration KPIs
- Monthly ride trends
- Time-of-day & day-of-week usage patterns
- Seasonality and rider type comparisons
- Member vs. Casual behavior breakdown

📥 Dashboard PDF: [`Cyclistic_Dashboard.pdf`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/Cyclistic_Dashboard.pdf)

---

## 📈 Key Insights
- ✅ Members ride more frequently, especially on weekdays and during commuting hours
- ✅ Casual riders take longer trips, mostly on weekends and afternoons
- ✅ Summer was the busiest season for total rides
- ✅ Classic bikes were the most popular among both user types

---

## 📁 Project Files
- [`cyclistic_analysis.R`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/cyclistic_analysis.R) – Data cleaning & processing in R  
- `cyclistic_cleaned_data.csv` – Final dataset used in Power BI  
- [`Cyclistic_Dashboard.pdf`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/Cyclistic_Dashboard.pdf) – Power BI dashboard  
- [`README.md`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/README.md) – This documentation

---

## 🧠 What I Learned
- Full-cycle analytics process: **ask → prepare → process → analyze → share → act**
- Practical data cleaning and feature extraction in R
- Building clean, insight-driven dashboards in Power BI
- Framing business insights to support decision-making

---

## 📬 Connect With Me
**Ahmed Salim**  
📍 Houston (Richmond), TX  
📧 [ahmedsabahsalim@gmail.com](mailto:ahmedsabahsalim@gmail.com)  
🔗 [LinkedIn: Ahmed Salim](https://www.linkedin.com/in/ahmed-s-salim/)  
🔗 [GitHub: Ahmed-S-Salim](https://github.com/Ahmed-S-Salim)

---

> ⚠️ *Note: This data is publicly available and modified for educational purposes only.*
