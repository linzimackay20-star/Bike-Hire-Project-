# Bike-Hire-Project-
## Coursera Bike Hire Project 
## Executive Summary: 
This project looks at how annual members and casual riders use Cyclistic bikes differently in order to discover insights that will help to inform marketing plans around increasing memberships. 
The dataset was cleaned and analysed using R, while summary tables and visualisations were produced in both R and Microsoft Excel. The analysis focused on 12 months of data -January 2024 to January 2025. I looked at daily and weekly ride data, station usage, and seasonal patterns. After identifying the most popular stations and days/months of the year to ride I discovered that: 
- The months June to October had the highest number of rides. 
- Members ride more Monday to Friday than they do on weekend’s which could suggest they are commuting. 
- Casual rides increase on a weekend and in the summer months and are longer rides times on average. This could suggest these rides are predominantly for leisure purposes.

I therefore made the following suggestions using data driven insights to improve membership signups:  
- Promote membership more heavily in the top 3 stations used by riders.
- Companies based around the most popular end stations for casual riders could be contacted to promote the membership scheme to potential commuters. 
-	Promotional campaigns could be stepped up in the busiest months.

## Business Problem 
How do annual members and casual riders use Cyclistic bikes differently? These insights will be used to create a new marketing strategy to convert casual riders into annual members.

## Stakeholders & data information: 
- Lily Moreno (Director of Marketing): Responsible for developing and executing marketing campaigns and evaluating marketing ROI.
- Cyclistic Marketing Analytics Team: Responsible for collecting and analysing ride data to guide marketing strategy.
- Cyclistic Executive Team: Responsible for approving strategic initiatives that support long-term company growth.

For the purposes of this case study, the data has been made available by Motivate International Inc. (under this license.) This is public data therefore data-privacy issues prohibit the usage of riders’ personally identifiable information. 

## Key Findings: 
-	65% of riders are members & 35% casual riders. 
-	The longest rides on average take place on a weekend (17 minutes) and the shortest rides mid-week Tues,Wed,Thurs (14 minutes).
-	Average ride length: members - 12 minutes and casual riders - 22 minutes with the longest rides taking place on a weekend. 
-	Weekdays were the most popular days for member rides suggesting they may be using the bikes to commute.
-	Rider numbers peak in the spring/summer months and slow in the autumn/winter months.
-	The top 3 most used stations are – Kingsbury St & Kinzie St, Navy Pier and DuSable Lake Shore Dr & Monroe St   

## Data cleaning:
-	Downloaded all relevant csv files (12x monthly spreadsheets) then used R to combine these into one merged database for the full year. 
-	Made all blanks NA so that they would still be counted. 
-	Formatted the the date/time format correctly and ensured they would show in the correct order for future analysis and visualisation. 
-	Checked all column names were formatted correctly. 
-	Reduced all decimal places to 2 to make data easier to read.
-	Checked for duplicate entries that could be removed but there weren’t any. 
-	Removed unrealistic ride times as they are likely to be errors and will affect the final analysis. This included rides lasting under 1 minute and exceeding 24 hours. 
-	Removed rides with missing date/time entries as these could not be used for analysis.
-	Added new columns for day of the week, ride length in minutes and month of the year.

## Analysis in R: 
-	Calculated the percentage of riders who are casual and who are members
-	Calculated rides per day both in total and by member and casual riders 
-	Calculated number of rides weekdays vs weekends
-	Analysed average ride length in minutes per day to see which days of the week people take the longest rides.
-	Created visuals using ggplot to show the outcomes of my analysis. Used the library(scales) function to update the graphs numerical value.
-	Calculated the top 3 most popular stations. 

## Analysis in Excel:
-	Created a table and graph to show rides per month in order to see which times of the year are most popular. 

## Recommendations:  
-	Promote membership more heavily in the top 3 stations used by riders : 
    - Kingsbury St & Kinzie St   
    - Navy Pier 
    - DuSable Lake Shore Dr & Monroe St.
-	Companies around the most popular end stations for casuals on week days could be contacted to promote the membership scheme to commuters. 
-	Promotional campaigns could be stepped up in the busiest months – June to October. 


## Future steps: 
-	There are a substantial amount of blanks in the station columns so it would be useful to have more information on these rides.
-	No personal data was provided so I cannot analyse how many rides each individual customer takes each week/month etc. This would be useful alongside data on costings. I could then analyse this to see how many casual riders are spending more a year on casual rides than they would if they joined the membership fee. 
