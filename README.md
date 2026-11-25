# 📊 UK Tech Conference – Post-Event Feedback Analysis

![Excel](https://img.shields.io/badge/Tool-Microsoft_Excel-217346?logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Tool-Power_Query-217346)
![Data Analytics](https://img.shields.io/badge/Field-Data_Analytics-blue)
![Project Status](https://img.shields.io/badge/Status-Completed-success)

## 1. Project Overview

This project focuses on cleaning, transforming and analysing post-event feedback collected from a series of UK technology conferences held across multiple cities.

The objective was to transform raw survey responses into a structured dataset and develop an Excel dashboard that provides meaningful insights into attendee experiences, event track performance and session participation.

Using Microsoft Excel, Power Query and PivotTables, I performed data preparation, handled missing values, created calculated columns, summarised feedback and developed visualisations to support evidence-based decision-making.

The project demonstrates an end-to-end data analytics workflow, from raw data preparation to insights and stakeholder recommendations.
<img width="878" height="586" alt="image" src="https://github.com/user-attachments/assets/3a86fda6-c87a-4c40-a307-347de0a243d5" />


## 2. Business Problem

Event organisers need reliable feedback to understand attendee experiences and improve future conferences.

However, raw survey data often contains inconsistent categories, missing values, incomplete feedback and other data quality issues that can affect analysis.

The key questions addressed in this project were:

- How can raw event feedback data be cleaned and prepared for analysis?
- How does attendee feedback vary across different UK cities?
- Which event tracks receive higher and lower average experience ratings?
- How does feedback participation vary by session type?
- What improvements can event organisers make based on the findings?

## 3. Project Objectives

The main objectives were to:

1. Clean and standardise the raw event feedback dataset.
2. Identify and remove exact duplicate records.
3. Handle missing Satisfaction and Experience Rating values.
4. Categorise experience ratings into meaningful groups.
5. Calculate the length of written feedback.
6. Analyse feedback by city, session type and event track.
7. Develop an interactive Excel dashboard.
8. Provide actionable recommendations to relevant stakeholders.

## 4. Tools and Technologies

| Tool | Application |
|---|---|
| Microsoft Excel | Data analysis and dashboard development |
| Power Query | Data cleaning and transformation |
| PivotTables | Data aggregation and analysis |
| Excel Charts | Data visualisation |
| Excel Slicers | Interactive filtering |

## 5. Dataset Description

The dataset contains post-event survey responses from a UK technology conference series.

**Original dataset:** `Event_Feedback_Responses`

**Number of original records:** 1,450

**Number of variables:** 10

### Dataset fields

| Column | Description |
|---|---|
| ResponseID | Unique response identifier |
| Attendee Name | Name of the attendee |
| City | City where the event was held |
| Event Track | Technology category |
| Session Type | Type of conference session |
| Response Channel | Channel used to submit feedback |
| Satisfaction | Attendee satisfaction category |
| Experience Rating | Numerical rating from 1 to 10 |
| Feedback | Written attendee comments |
| Submitted On | Date feedback was submitted |

### Dataset coverage

- 15 UK cities
- 5 event tracks
- 4 session types
- Survey submission period: 19 April 2025 – 19 July 2025

## 6. Data Cleaning and Transformation

The raw dataset was imported into Power Query, where the following operations were performed:

### Step 1: Import Data

Imported the `Event_Feedback_Responses` worksheet into Power Query for data preparation.

### Step 2: Standardise Categories

Applied Proper Case formatting to:

- Event Track
- Session Type

This ensured consistency across categorical values.

### Step 3: Remove Duplicates

Checked for exact duplicate records using all columns.

No exact duplicate records were identified in the original dataset.

### Step 4: Handle Missing Satisfaction Values

Filtered out records with blank Satisfaction scores to ensure that the satisfaction analysis was based on available responses.

### Step 5: Handle Missing Experience Ratings

Replaced missing Experience Rating values using the average rating for the corresponding Event Track.

This approach retained records with missing numerical ratings while using track-level averages as estimates.

### Step 6: Create Rating Categories

Added a calculated column called `Rating Category` using the following classification:

| Experience Rating | Category |
|---|---|
| 8–10 | Excellent |
| 5–7 | Okay |
| 1–4 | Poor |

### Step 7: Calculate Feedback Length

Created a `Feedback Length` column to calculate the number of words in each written feedback response.

This provides an additional measure for exploring written feedback patterns.

### Step 8: Load Cleaned Data

Loaded the transformed dataset back into Excel for further analysis using PivotTables and charts.

## 7. Data Cleaning Results

| Data Quality Metric | Result |
|---|---:|
| Original records | 1,450 |
| Final cleaned records | 1,001 |
| Blank Satisfaction records excluded | 449 |
| Exact duplicates identified | 0 |
| Missing Experience Ratings in raw data | 61 |
| Missing Feedback fields remaining | 101 |

The final dataset contained 1,001 records after filtering out responses with blank Satisfaction values.

## 8. Data Analysis and PivotTables

Two main analytical summaries were developed.

### Analysis 1: Feedback Entries by City and Session Type

A PivotTable was created to count feedback entries across different cities and session types.

The analysis covered:

- Keynote
- Lightning Talk
- Panel
- Workshop

This provides a breakdown of feedback participation across the 15 cities.

### Analysis 2: Average Experience Rating by Event Track

A second PivotTable was created to calculate the average Experience Rating for each event track.

The five tracks analysed were:

- AI & Data
- Cloud Computing
- Cybersecurity
- Devops
- Web Development

## 9. Key Findings

### Overall Findings

| Indicator | Result |
|---|---:|
| Total original responses | 1,450 |
| Cleaned responses | 1,001 |
| Cities analysed | 15 |
| Event tracks analysed | 5 |
| Session types analysed | 4 |
| Overall average experience rating | 5.58/10 |

### Average Experience Rating by Event Track

| Event Track | Average Rating |
|---|---:|
| AI & Data | 5.69 |
| Cloud Computing | 5.63 |
| Devops | 5.62 |
| Cybersecurity | 5.59 |
| Web Development | 5.33 |

**Key observations:**

- AI & Data recorded the highest average experience rating at 5.69.
- Web Development recorded the lowest average experience rating at 5.33.
- The average ratings across all five tracks were relatively close.
- The overall average experience rating was 5.58 out of 10.

These results highlight areas that may require further investigation to understand attendee experiences.

## 10. Dashboard and Visualisations

The Excel dashboard was developed to communicate the findings in a clear and accessible format.

The dashboard includes:

- Feedback entries by City and Session Type.
- Average Experience Rating by Event Track.
- City filtering using slicers.
- Visual summaries of attendee feedback.

### Visualisation 1: Average Experience Rating by Event Track

![Average Experience Rating by Event Track](average_rating_by_track.png)

### Visualisation 2: Feedback Entries by City and Session Type

![Feedback Entries by City and Session Type](feedback_by_city_and_session.png)

The visualisations help stakeholders compare event track performance and understand feedback distribution across cities and session formats.

## 11. Recommendations to Stakeholders

Based on the findings, the following recommendations are proposed:

### 1. Event Organisers and Conference Management

- Review the overall attendee experience, particularly the average rating of 5.58/10.
- Investigate factors contributing to lower satisfaction.
- Improve event planning, communication, scheduling and attendee engagement.
- Establish measurable satisfaction targets for future conferences.

### 2. Programme Managers and Track Leads

- Investigate why Web Development recorded the lowest average rating of 5.33.
- Review session content, speaker delivery and practical relevance.
- Identify effective practices from higher-rated tracks such as AI & Data.
- Introduce improvements based on attendee feedback.

### 3. Regional Event Coordinators

- Compare feedback across the 15 cities.
- Investigate differences in attendee experiences.
- Review venue accessibility, registration processes and event logistics.
- Share successful practices across regional teams.

### 4. Speakers and Session Facilitators

- Use attendee comments to improve presentation quality.
- Introduce more practical demonstrations and interactive discussions.
- Improve the balance between technical depth and accessibility.
- Monitor feedback after future sessions.

### 5. Data and Evaluation Teams

- Improve survey completion rates.
- Reduce missing values in future data collection.
- Monitor attendee satisfaction trends over time.
- Distinguish actual ratings from imputed ratings in analytical reporting.
- Maintain consistent performance indicators across future events.

### Expected Benefits

Implementing these recommendations could help stakeholders improve attendee satisfaction, strengthen conference programmes, allocate resources more effectively and establish a continuous improvement process.

Further investigation is needed to establish the specific factors influencing attendee satisfaction.

## 12. Limitations and Considerations

A few considerations should be taken into account when interpreting the findings:

- The analysis is based on submitted survey responses and may not represent every conference attendee.
- Missing Experience Rating values were replaced using event track averages, which may influence the calculated averages.
- Written feedback was incomplete for 101 records.
- The analysis identifies descriptive patterns but does not establish the causes of satisfaction differences.
- Further analysis of written comments and individual session performance could provide additional insights.

## 13. Future Improvements

Potential extensions of this project include:

- Developing a weekly feedback submission trend.
- Adding a timeline to analyse submission dates.
- Introducing additional dashboard slicers.
- Performing sentiment analysis on written feedback.
- Comparing satisfaction across individual sessions and cities.
- Developing automated reporting using Power BI.
- Monitoring changes in attendee satisfaction across future conference editions.

## 14. Skills Demonstrated

Through this project, I demonstrated practical skills in:

- Data cleaning and preparation
- Power Query transformations
- Missing-value treatment
- Data standardisation
- Calculated columns
- PivotTable analysis
- Data aggregation
- Data visualisation
- Excel dashboard development
- Business insights and stakeholder recommendations

## 15. Project Conclusion

This project demonstrates how Microsoft Excel and Power Query can be used to transform raw survey data into structured information that supports decision-making.

By combining data cleaning, analytical summaries and visualisations, I was able to identify patterns in attendee feedback, compare event track ratings and develop recommendations for conference stakeholders.

The experience strengthened my understanding of the complete data analytics process and reinforced the importance of data quality, analytical thinking and effective communication of findings.

---

**Author:** https://github.com/joshuamakula/

**Tools:** Microsoft Excel | Power Query | PivotTables | Excel Dashboard

**Project Category:** Data Cleaning, Exploratory Data Analysis and Data Visualisation

**Feedback and Contributions:** Suggestions and constructive feedback are welcome.
