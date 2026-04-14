# Panic-Attacks-Risk-Analysis
This project explores behavioral and lifestyle factors associated with panic attacks using an interactive Power BI dashboard. The analysis focuses on identifying patterns between sleep duration, panic severity, and other health indicators to support data-driven mental health insights.
## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Data Source](#data-source)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Data Modeling](#data-modeling)
- [Dashboard Pages & Features](#dashboard-pages--features)
- [Insights](#insights)
- [Executive Recommendations](#executive-recommendations)
- [Tools & Technologies](#tools--technologies)

## Project Overview
Panic attacks can be influenced by multiple behavioral and physiological factors. This dashboard analyzes a healthcare dataset to understand how variables such as sleep duration, panic duration, and lifestyle indicators relate to panic attack severity.

The goal is to help identify potential risk patterns that may assist healthcare professionals in understanding patient conditions and early risk indicators.

## Problem Statement
Understanding panic attack patterns requires analyzing multiple behavioral indicators. This project investigates:

- Distribution of panic severity among patients

- Relationship between sleep duration and panic scores

- Proportion of high-risk patients

- Average panic attack duration and behavioral trends

- The dashboard aims to highlight patterns that may indicate elevated panic risk.

## Data Source
Healthcare dataset containing behavioral and lifestyle attributes of patients experiencing panic attacks.

Key attributes include:

- Panic Score (Low, Medium, High)

- Sleep Hours

- Panic Attack Duration

- Medical History

- Trigger Reason

- Lifestyle Indicators

## Data Cleaning & Preparation
Data preparation was performed using Power Query.

Steps included:

- Data type corrections
- Handling missing values
- Creating calculated columns
- Categorizing sleep duration
- Preparing panic score classifications

## Data Modeling 
Data Modeling

A structured data model was built to support efficient analysis.

Techniques used:

- Calculated columns
- DAX measures
- Aggregation metrics
- Behavioral categorization logic

Example measures created:
- High Risk Patient Ratio
- Average Panic Duration
- Average Sleep Hours
- Total Patients


## Dashboard Pages & Features
### 1. Executive_page
<img width="1294" height="722" alt="image" src="https://github.com/user-attachments/assets/5f370a4a-3c1a-42b4-a7eb-2819d8f0df57" />
Features:

- KPI Cards: Total Patients, High-Risk Patients, Avg Sleep Hours, Avg Panic Duration
→ Provide quick snapshot of population size, risk concentration, and key behavioral indicators
- Donut Chart (Panic Score Distribution):
→ Used to show proportion of Low, Medium, High risk segments clearly for quick comparison
- Gauge Chart (High-Risk Ratio):
→ Highlights % of high-risk patients against total population to emphasize severity level
- Clustered Column Chart (Panic Score vs Sleep Duration):
→ Helps analyze relationship between sleep patterns and panic severity across segments
- Key Insights Panel:
→ Summarizes critical patterns for decision-makers without requiring deep chart analysis


### 2.No. of patients by symptom 
<img width="1311" height="730" alt="image" src="https://github.com/user-attachments/assets/0f010164-a1ea-415f-8d77-b2468474c6e9" />

Features:

- Bar Charts (Symptom-wise Distribution):
→ Separate bars for dizziness, chest pain, sweating, shortness of breath, trembling
→ Used to compare frequency of each symptom across patients (True vs False)
- Binary Comparison (True vs False split):
→ Helps identify which symptoms are more prevalent and reliable as indicators
- Visual Layout (Multi-panel design):
→ Enables side-by-side comparison of symptoms for faster pattern recognition
- Illustrative Background Layer:
→ Enhances storytelling and aligns with mental health theme (without affecting data readability)

### 3. Other Requirements
<img width="1281" height="720" alt="image" src="https://github.com/user-attachments/assets/dc4745be-ba9d-41c0-bba1-cd714760479b" />
Features:

- Slicers (Dynamic Filtering): Panic Score (H/M/L), Gender, Trigger Reason, Medical History
→ Enables multi-dimensional filtering to analyze how different behavioral and demographic factors impact panic patterns
- Area/Line Charts (Sleep Hours Distribution):
→ Used to visualize patient distribution across sleep duration, helping identify concentration patterns and irregularities
- Area/Line Charts (Panic Attack Duration):
→ Captures variation in attack duration across patients, useful for identifying severity spread
- Area Chart (Drinks per Week):
→ Shows distribution of alcohol consumption to analyze its potential behavioral impact on panic frequency
- Interactive Cross-Filtering:
→ Selecting any slicer dynamically updates all visuals, allowing deeper cohort-level analysis (e.g., high-risk + caffeine-triggered patients)

## Insights
- ~20% of patients fall into the high-risk category, with risk concentrated among individuals showing behavioral and lifestyle imbalances
- Sleep deprivation (≤5–6 hours) emerges as the strongest consistent indicator of higher panic severity and frequency
- Behavioral factors such as high caffeine intake and alcohol consumption are positively associated with longer and more frequent panic attacks
- Multi-symptom presence (shortness of breath, sweating, trembling) is more common in high-risk patients, making combined symptoms a stronger predictor than isolated ones
- Pre-existing conditions (anxiety/depression) combined with specific triggers (phobia/caffeine) significantly amplify risk, enabling targeted cohort    identification for intervention


## Executive Recommendations
- Implement early risk screening using behavioral indicators (sleep <6 hrs, high caffeine/alcohol intake) to proactively identify high-risk patients
- Prioritize intervention programs for high-risk cohorts (~20%), focusing on patients with multiple symptoms and pre-existing conditions (anxiety/depression)
- Design targeted awareness and lifestyle management plans (sleep hygiene, caffeine reduction) to reduce panic severity at an early stage
- Leverage symptom clustering for faster diagnosis, using combinations like shortness of breath + sweating as key screening triggers
- Enable continuous monitoring dashboards for clinicians, allowing real-time tracking of high-risk patients and timely intervention decisions

## Tools & Technologies
- Data Analysis & Processing: Python (Pandas, NumPy)
- Data Querying: SQL (PostgreSQL)
- Data Visualization & BI: Power BI (DAX, Power Query)
