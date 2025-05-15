# STEP 0: Install Packages (Run Once)
#-----------------------------
install.packages("tidyverse")   # Data wrangling & visualization
install.packages("lubridate")   # Working with dates
install.packages("hms")         # Working with time (HH:MM:SS)
install.packages("data.table")  # Exporting clean data to CSV

#-----------------------------
# STEP 1: Load Libraries
#-----------------------------
library(tidyverse)
library(lubridate)
library(hms)
library(data.table)

#-----------------------------
# STEP 2: Load 12-Month CSV Files (Apr 2024 - Mar 2025)
#-----------------------------
apr <- read_csv("202404-divvy-tripdata.csv")
may <- read_csv("202405-divvy-tripdata.csv")
jun <- read_csv("202406-divvy-tripdata.csv")
jul <- read_csv("202407-divvy-tripdata.csv")
aug <- read_csv("202408-divvy-tripdata.csv")
sep <- read_csv("202409-divvy-tripdata.csv")
oct <- read_csv("202410-divvy-tripdata.csv")
nov <- read_csv("202411-divvy-tripdata.csv")
dec <- read_csv("202412-divvy-tripdata.csv")
jan <- read_csv("202501-divvy-tripdata.csv")
feb <- read_csv("202502-divvy-tripdata.csv")
mar <- read_csv("202503-divvy-tripdata.csv")

# Combine all data into one big data frame
bike_data <- rbind(apr, may, jun, jul, aug, sep, oct, nov, dec, jan, feb, mar)

# Clear memory by removing monthly variables
rm(apr, may, jun, jul, aug, sep, oct, nov, dec, jan, feb, mar)

#-----------------------------
# STEP 3: Clean and Filter Data
#-----------------------------
# Calculate ride length (in minutes)
bike_data$ride_length <- difftime(bike_data$ended_at, bike_data$started_at, units = "mins")

# Keep only valid rides (greater than 0 mins)
bike_data <- bike_data %>% filter(ride_length > 0)

# Remove missing data and duplicates
bike_data <- na.omit(bike_data)
bike_data <- distinct(bike_data)

# Drop columns we don't need
bike_data <- bike_data %>%
  select(-c(ride_id, start_station_id, end_station_id,
            start_lat, start_lng, end_lat, end_lng))

#-----------------------------
# STEP 4: Add Date & Time Features
#-----------------------------
bike_data <- bike_data %>%
  mutate(
    date = as.Date(started_at),
    day_of_week = format(date, "%A"),
    month = format(date, "%m"),
    day = format(date, "%d"),
    year = format(date, "%Y"),
    hour = hour(started_at),
    time_of_day = case_when(
      hour < 6 ~ "Night",
      hour < 12 ~ "Morning",
      hour < 18 ~ "Afternoon",
      TRUE ~ "Evening"
    ),
    season = case_when(
      month %in% c("12", "01", "02") ~ "Winter",
      month %in% c("03", "04", "05") ~ "Spring",
      month %in% c("06", "07", "08") ~ "Summer",
      month %in% c("09", "10", "11") ~ "Fall"
    )
  )

#-----------------------------
# STEP 5: Basic Summary & Insights
#-----------------------------

# Total number of rides
nrow(bike_data)

# Rides by member type
bike_data %>% count(member_casual)

# Rides by bike type
bike_data %>% count(rideable_type)

# Average ride length overall
mean(bike_data$ride_length)

# Average ride length by rider type
bike_data %>%
  group_by(member_casual) %>%
  summarise(avg_duration = mean(ride_length))

#-----------------------------
# STEP 6: Explore Ride Trends
#-----------------------------

# Rides by hour of day
bike_data %>% count(hour, member_casual)

# Rides by day of the week
bike_data %>% count(day_of_week, member_casual)

# Rides by time of day
bike_data %>% count(time_of_day, member_casual)

# Rides by season
bike_data %>% count(season, member_casual)

#-----------------------------
# STEP 7: Save Cleaned Data
#-----------------------------
# Export to CSV for dashboard or future use
fwrite(bike_data, "cyclistic_cleaned_data.csv")
