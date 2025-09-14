# Project Background
Dataset: https://www.kaggle.com/datasets/swaptr/layoffs-2022

## Context
Tech firms around the globe are fighting the economic slowdown. The slow consumer spending, higher interest rates by central banks and strong dollars overseas are hinting towards possible recession and tech firms have started laying employees off. This economic slowdown has made Meta recently fire 13% of its workforce, which amounts to more than 11,000 employees.

The dataset contains information on **company name**, **industry, location**, **total layoffs**, **percentage of workforce laid off**, **funding raised**, **company stage**, and **dates of layoffs**. The goal of this analysis is to provide **actionable insights on workforce reductions** and **identify patterns across industries, company sizes, and stages**.

## Content
Tracking the tech layoffs reported on the following platforms:

* Bloomberg
* San Francisco Business Times
* TechCrunch
* The New York Times

The data availability is from when COVID-19 was declared as a pandemic i.e. 11 March 2020 to present (21 Apr 2025).

## Key Areas
Insights and recommendations are provided on the following key areas:

- **Category 1: Industry-level layoff trends**

Analysis of which industries have the highest total layoffs and highest average % of employees laid off.
- **Category 2: Company size and funding impact**

Understanding how layoffs differ across companies with different funding levels (Small, Medium, Large) and workforce sizes. 

- **Category 3: Company stage and temporal trends**

Insights on how layoffs vary by company stage (Series B–H, Post-IPO, Acquired) and over time.
- **Category 4: Geographic and regional patterns**

Analysis of layoffs by country and region to identify markets with higher workforce reduction risk.

# Data Structure
The dataset for this project consists of one primary table that tracks layoffs across multiple companies worldwide.

- company (TEXT): Name of the company.
- industry (TEXT): Industry the company operates in (e.g., Tech, Retail, Healthcare).
- location (TEXT): City or region of the company.
- country (TEXT): Country where the company is based.
- total_laid_off (INT): Total number of employees laid off during the period.
- percentage_laid_off (DECIMAL): Fraction of the company workforce laid off (e.g., 0.06 = 6%).
- date (DATE): Date when layoffs were reported. 
- stage (TEXT): Company stage: Series B–H, Post-IPO, Acquired, Private Equity.
- funds_raised_millions (INT): Total funds raised by the company in millions USD.

# Executive Summary

## Overview of Findings
1. Industry-specific layoff trends: Certain industries, such as **Food, Travel, and Real Estate**, experienced **significantly higher layoff percentages**, while others like **Finance and Other sectors** maintained more **stable workforce levels**. 
2. Company size and funding matter: Companies with larger funding or more mature stages (Series D–H, Post-IPO) generally had lower percentages of layoffs, suggesting that financial stability and maturity provide a buffer against workforce reductions.
3. Temporal and regional patterns: Layoffs show month-to-month variation, with some countries like the United States and India reporting the highest total layoffs. This indicates that both timing and location are key factors for workforce planning and risk mitigation.

## Insights and Recommendations
**Category 1: Industry-level Layoff Trends**
- Industries such as Food, Travel, and Real Estate show the highest average percentage of layoffs, while industries like Finance and Other sectors maintain more stable workforce levels.
- Bar charts show that top layoffs by total employees also align with these high-risk industries.

<img width="600" height="544" alt="image" src="https://github.com/user-attachments/assets/8535c2f2-2505-48c5-9565-e0fdfb4f3be9" />

**Category 2: Company size and funding impact**
- Companies with larger funding (>200M USD) and more mature stages (Series D–H, Post-IPO) generally show lower percentage layoffs.
- Smaller or early-stage companies (low funding, <50M) often have higher layoffs, with some exceeding 30% of the workforce.
  
<img width="600" height="544" alt="image" src="https://github.com/user-attachments/assets/e2a7b216-b17b-454d-abb6-0aa8ac999787" />

**Category 3: Company Stage & Temporal Trends**
- Layoffs fluctuate across months, with peaks in certain periods, indicating seasonal or event-driven workforce reductions.
- Post-IPO and late-stage companies are less affected, while early-stage and Series B–C companies are more sensitive to funding or market pressures.

<img width="600" height="546" alt="image" src="https://github.com/user-attachments/assets/7103d2ae-cd77-458e-904e-fdde1eff4d0c" />

**Category 4: Geographic and Regional Patterns**
- Countries such as the United States and India report the highest total layoffs, while smaller markets have fewer but sometimes higher percentages per company.
- This could be explained as the US is the world’s largest tech & startup hub, so naturally it dominates both in company count and layoff volume. India is the second largest in scale, as India has many large IT services & outsourcing firms (Infosys, Wipro, TCS).
- Regional differences may be linked to industry concentration, local regulations, and funding availability.

<img width="700" height="555" alt="image" src="https://github.com/user-attachments/assets/12518fe3-01a1-4e6b-85bf-c10813620c46" />



