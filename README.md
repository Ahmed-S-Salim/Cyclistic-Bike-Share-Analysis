# 🚴 Cyclistic Bike-Share Analysis – Capstone Project

**Author:** Ahmed Salim  
**Level:** Beginner – Google Data Analytics Certificate Project  
**Tools Used:** R, RStudio (Tidyverse, Lubridate, HMS, Data.table), Excel, Power BI  
**GitHub Repo:** [Cyclistic-Bike-Share-Analysis](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis)  
**Kaggle Dataset:** [Cyclistic Bike-Share Capstone Project](https://www.kaggle.com/datasets/ahmedssalim/cyclistic-bike-share-analysis-capstone-project-a)

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
- **Source:** Divvy Bike System – [https://divvybikes.com/system-data](https://divvybikes.com/system-data)  
- **Provider:** Motivate International Inc.  
- **Timeframe:** April 2024 to March 2025  
- **Files:** 12 monthly `.csv` files  
- **Volume:** 5M+ ride records  
- **Cleaned Dataset on Kaggle:** [View Here](https://www.kaggle.com/datasets/ahmedssalim/cyclistic-bike-share-analysis-capstone-project-a)

---

## ⚠️ Disclaimer
> This data is provided “as-is” and has been modified for educational purposes only.  
> All ride data is owned by Motivate International Inc. and Divvy Bikes.  
> Redistribution or commercial use is not permitted.

---

## 🛠️ Tools & Skills Used
- **RStudio** – Scripting environment  
- **Tidyverse** – Wrangling and analysis (`dplyr`, `ggplot2`, `readr`)  
- **Lubridate** – Date/time parsing  
- **HMS** – Time-of-day classification  
- **Data.table** – Fast CSV export  
- **Excel** – Data review and QA  
- **Power BI** – Visualization dashboard

---

## 🧼 Data Cleaning Summary (R)
- Combined 12 monthly `.csv` files using `rbind()`  
- Removed:
  - Rows with missing or null values  
  - Duplicate records  
  - Rides with zero or negative duration  
- Engineered columns:
  - `ride_length` in minutes  
  - `day_of_week`, `hour`, `season`, and `time_of_day`

📄 R Script: [`cyclistic_analysis.R`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/cyclistic_analysis.R)

---

## 📊 Dashboard Note
After completing the analysis and designing the dashboard in **Power BI**, I discovered that Power BI Public does not support sharing `.pbix` files or dashboards from the free version.  
➡️ To ensure insights remain accessible, I exported the dashboard as a **PDF report**, which includes all visuals, charts, and KPIs.

📄 Power BI Report: [`Cyclistic_Dashboard.pdf`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/Cyclistic_Dashboard.pdf)

---

## 📈 Key Insights
- ✅ Members ride more frequently—mostly on weekdays and commuting hours  
- ✅ Casual riders take longer trips—mostly on weekends and afternoons  
- ✅ Summer had the highest overall ride volume  
- ✅ Classic bikes are the most used type across both rider groups

---

## 📁 Project Files
- [`cyclistic_analysis.R`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/cyclistic_analysis.R) – Full cleaning and prep script  
- [`cyclistic_cleaned_data.csv`](https://www.kaggle.com/datasets/ahmedssalim/cyclistic-bike-share-analysis-capstone-project-a) – Final dataset used for visualizations  
- [`Cyclistic_Dashboard.pdf`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/Cyclistic_Dashboard.pdf) – Power BI dashboard  
- [`README.md`](https://github.com/Ahmed-S-Salim/Cyclistic-Bike-Share-Analysis/blob/main/README.md) – Project summary and documentation

---

## 🧠 What I Learned
- End-to-end workflow of a real-world analytics project  
- Practical use of R and Tidyverse for data wrangling  
- How to extract actionable insights from raw data  
- Designing clear visual narratives using Power BI  
- Writing and documenting projects for employers and portfolio

---

## 📬 Connect With Me
**Ahmed Salim**  
📍 Houston (Richmond), TX  
📧 [ahmedsabahsalim@gmail.com](mailto:ahmedsabahsalim@gmail.com)  
🔗 [LinkedIn: Ahmed Salim](https://www.linkedin.com/in/ahmed-s-salim/)  
🔗 [GitHub: Ahmed-S-Salim](https://github.com/Ahmed-S-Salim)

---

> ⚠️ *Note: This dataset is for educational use only and should not be used for commercial purposes.*
