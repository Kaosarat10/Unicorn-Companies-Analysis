# **Unicorn Analysis**

## **Table of Contents**

1. [Introduction](#introduction)  
2. [Project Description](#project-description)  
3. [Project Aim](#project-aim)  
4. [About the Dataset](#about-the-dataset)  
5. [Importing the Dataset to Excel](#importing-the-dataset-to-excel)  
6. [Preparation of the Dataset: Cleaning and Transforming](#preparation-of-the-dataset-cleaning-and-transforming)  
7. [Data Modeling in Excel](#data-modeling-in-excel)  
8. [Data Analysis in Excel](#data-analysis-in-excel)  
9. [Data Visualization in Excel](#data-visualization-in-excel)  
10. [Insights from the Data Analysis](#insights-from-the-data-analysis)  
11. [Recommendations from the Data Analysis](#recommendations-from-the-data-analysis)  
12. [Conclusion](#conclusion)  

---

## **Introduction**

This project focuses on analyzing billion-dollar unicorn companies using Microsoft Excel. The goal is to identify key trends in the startup ecosystem, such as investment patterns, industry dominance, and geographical distribution of unicorns. 

## **Project Description**

Unicorn companies are private firms valued at $1 billion or more. This project aims to analyze their growth patterns, return on investment (ROI), investor influence, and regional distribution. The dataset, sourced from Maven Analytics, contains information on 1,074 unicorn companies, including valuation, funding, country of origin, industry, select investors, and the years they were founded and became unicorns.

## **Project Aim**

The main objective of this project is to analyze billion-dollar unicorn companies and answer key business questions:

✅ Which unicorn companies have had the highest return on investment?  
✅ How long does it take for a startup to achieve unicorn status?  
✅ Which countries and cities produce the most unicorns?  
✅ Who are the biggest investors funding these startups?  

## **About the Dataset**

The dataset contains 1,074 rows and 10 columns:

- **Company** – Name of the unicorn company.
- **Valuation** – The company's valuation in billions of dollars.
- **Date Joined** – The date the company achieved unicorn status.
- **Industry** – The sector in which the company operates.
- **City** – The city where the company is headquartered.
- **Country** – The country of origin.
- **Continent** – The geographical region of the company.
- **Year Founded** – The year the company was established.
- **Funding** – Total funding received by the company.
- **Select Investors** – Major investors backing the company.

## **Importing the Dataset to Excel**

The dataset was imported as a CSV file into Excel. A duplicate copy was created before launching Power Query for transformation.

## **Preparation of the Dataset: Cleaning and Transforming**

- **Removed Duplicates**  
- **Assigned Correct Data Types**  
- **Added 'Years to Unicorn' Column**  
- **Split Investors into Multiple Columns**  
- **Duplicated 'Date Joined' and Extracted Year**  
- **Standardized Funding Column to Billions** using:

```excel
=IF(RIGHT(A2,1)="B", LEFT(A2,LEN(A2)-1)*1, LEFT(A2,LEN(A2)-1)/1000)
```

## **Data Modeling in Excel**

- **Created a Fact Table Named Unicorn Dataset**  
- **Created a Dimension Table Named Companies**  
- **Added Data to the Model**  
- **Built Relationships Between Tables**  

## **Data Analysis in Excel**

Key performance indicators (KPIs) analyzed:

- **Average Return on Investment (ROI)**
- **Average Years to Unicorn**
- **Total Number of Unicorn Companies**
- **Total Number of Investors**

## **Data Visualization in Excel**
Two dashboards were created: an **Overview Dashboard** and an **Insights Dashboard**.

### **Overview Dashboard**
- **KPI Cards**: Avg ROI, Avg Years to Unicorn, Total Unicorn Companies, Total Investors.
- **Bar Chart**: Top 10 Investors in Unicorn Companies.
- **Line Chart**: Time Taken to Reach Unicorn Status.
- **Lollipop Chart**: Top 5 Unicorn Companies by ROI.
- **Map**: Countries Producing the Most Unicorns.

### **Insights Dashboard**
- **Bar Chart**: Top Industries by ROI.
- **Bar Chart**: Top Cities by ROI.
- **Bar Chart**: Top 5 Investors.
- **Bar Chart**: Average Years to Unicorn by Industry.
- **Bar Chart**: Top 5 Industries by Investment.
- **Bar Chart**: Top Cities with the Most Unicorns.
- **Slicer**: Continent filter for dynamic analysis.

- ### **View Dashboards**
- [Overview Dashboard](#)  
- [Insights Dashboard](#)  

## **Insights from the Data Analysis**

- **Industries with the Highest ROI**: Fintech, Mobile & Telecommunications, and Hardware lead in ROI performance.
- **Industries with the Most Investment**: Fintech, Internet & Software Services, E-Commerce, and AI attract the highest funding.
- **Top Investors**: Sequoia Capital China, Accel, Andreessen Horowitz, and Insight Partners are the most active investors.
- **Top Unicorn Companies by ROI**: Zwift, Dunamu, Pilot.com, Bought By Many, Domestika, and DJI Innovations.
- **Countries Producing the Most Unicorns**: United States (554), China (169), and India (65).
- **Top Cities for Unicorns**: London, Shanghai, Beijing, New York, and San Francisco.
- **Average Years to Unicorn**: The average time it takes for a company to reach unicorn status is 7.5 years.

## **Recommendations from the Data Analysis**

- **For Investors**: Focus on fintech, telecommunications, and AI startups, as they show high ROI potential.
- **For Startups**: Companies should aim for strategic funding rounds, as unicorns typically achieve this status in 7.5 years.
- **For Policymakers**: Supporting startups in the United States, China, and India could further boost unicorn formation.
- **For Entrepreneurs**: Consider launching in cities like London, Shanghai, and San Francisco, which have thriving startup ecosystems.

## **Conclusion**

This project successfully analyzed unicorn companies, highlighting investment trends, high-performing industries, and key investor activities. The insights derived can help stakeholders make informed decisions in the startup ecosystem.
