Author: Ahmed SalimLevel: Beginner – Google Data Analytics Certificate ProjectTools Used: R, RStudio (Tidyverse, Lubridate, HMS, Data.table), Excel, Power BI

📌 Project Overview

This project is the final capstone for the Google Data Analytics Professional Certificate. The goal is to help Cyclistic, a fictional bike-share company in Chicago, understand how casual riders and annual members use their service differently. By identifying usage patterns, the company can develop strategies to convert more casual riders into loyal, long-term members.

🌟 Business Task

Objective:Analyze 12 months of historical ride data to answer:"How do casual riders and annual members use Cyclistic bikes differently?"

The final insights will support the Cyclistic marketing team’s goal of increasing membership.

📂 Data Source

The data was provided by Motivate International Inc. and made public through the Divvy bike-share system.

Date range: April 2024 to March 2025

Files: 12 monthly .csv files

Size: Over 5 million rows of ride-level data

🔧 Tools & Skills Used

R: Data cleaning, transformation, summarization

Tidyverse: dplyr, ggplot2, readr, tidyr for data wrangling

Lubridate: Date & time manipulation

HMS: Time-of-day classification

Data.table: Export cleaned dataset

Excel: Exploratory review and quick summaries

Power BI: Interactive dashboard design and data visualization

RStudio: Environment for running and testing all code

🧼 Data Cleaning Steps

Combined 12 months of ride data using rbind()

Removed missing and duplicate rows

Created a ride_length column (in minutes)

Filtered out rides with zero or negative duration

Dropped unnecessary columns (IDs and GPS coordinates)

Extracted features: date, time, day of week, season, hour, and time of day

📄 R Script: cyclistic_analysis.R

📈 Key Insights

Members ride more frequently than casual users.

Casual riders take longer rides on average.

Casual users ride more on weekends and afternoons.

Members are more active during weekday mornings and commute hours.

Classic bikes are the most commonly used type across both groups.

📊 Dashboard & Deliverables

Visualizations created in Power BI

Dashboard exported as PDF for sharing

Highlights ride trends, seasonality, rider behavior, and key comparisons

PDF File: Cyclistic_Dashboard.pdf

📁 Project Files

cyclistic_analysis.R – Full R script

cyclistic_cleaned_data.csv – Cleaned dataset for dashboard use

Cyclistic_Dashboard.pdf – Power BI dashboard exported as PDF

README.md – Project documentation

🧐 What I Learned

How to apply the full data analysis process: ask, prepare, process, analyze, share, and act.

Gained hands-on experience in data cleaning, and summary statistics in R.

Learned how to create business-driven insights that can help decision-making.

📩 Connect with Me

Ahmed Salim📍 Houston (Richmond), TX📧 ahmedsabahsalim@gmail.com🔗 LinkedIn: Ahmed Salim

⚠️ This data is for educational purposes only and has been altered to protect user privacy.

