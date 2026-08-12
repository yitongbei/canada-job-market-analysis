# Canada Job Market Analysis

## Overview

This project analyzes labour market trends across five Canadian geographies using Statistics Canada data. The analysis focuses on job vacancy rates and average offered hourly wages from 2015Q1 to 2026Q1.

The five selected geographies are:

* Canada
* Ontario
* Ottawa, Ontario
* Toronto, Ontario
* Montréal, Quebec

## Data Source

**Statistics Canada — Table 14-10-0441-01**

The dataset contains quarterly information on:

* Job vacancies
* Job vacancy rate
* Payroll employees
* Average offered hourly wage

The raw data were cleaned, reshaped, and filtered to create a consistent five-region comparison dataset.

## Tools

* Python
* pandas
* matplotlib
* Google Colab / Jupyter Notebook

## Analysis

The project includes:

* Initial data inspection and cleaning
* Geographic identifier and duplicate checks
* Missing-value analysis
* Long-to-wide data reshaping
* Latest-quarter comparison
* Ottawa-specific labour market analysis
* Historical job vacancy rate comparison
* Historical offered hourly wage comparison
* Trend visualizations across the five selected regions

## Key Findings

* Ottawa recorded the highest historical job vacancy rate among the five selected regions, reaching **6.3% in 2022Q2**.
* From the earliest available observations to 2026Q1, job vacancy rates declined in **Ontario, Ottawa, and Toronto**, remained unchanged in **Canada**, and increased in **Montréal**.
* Toronto had the highest average offered hourly wage in **2026Q1 at $32.80 per hour**.
* Toronto recorded the largest absolute wage increase from 2015Q1 to 2026Q1, increasing by **$12.50 per hour**.
* Ottawa recorded the largest percentage wage increase over the same period, at **62.2%**.

## Visualizations

The notebook includes two main historical trend charts:

1. **Job Vacancy Rate Trends Across Five Regions, 2015Q1–2026Q1**
2. **Average Offered Hourly Wage Trends Across Five Regions, 2015Q1–2026Q1**

These visualizations show how labour demand and offered wages evolved across the selected regions over time.

## Data Notes and Limitations

Three missing observations occur for Ottawa, Ontario in 2015Q1. These values are retained as missing rather than replaced with zero because missing or unpublished data do not imply a true value of zero.

Average offered hourly wage values are **nominal and are not adjusted for inflation**. Therefore, nominal wage growth should not be interpreted as equivalent growth in purchasing power.

Job vacancy counts should also be interpreted cautiously when comparing geographies of substantially different sizes. Job vacancy rates provide a more meaningful relative comparison.

## Running the Notebook

The notebook expects the Statistics Canada CSV file to be available as:

`14100441.csv`

Place the CSV file in the same working directory as the notebook before running it.

Then run:

`Canada_Job_Market_Analysis.ipynb`

from top to bottom.

## Repository Contents

* `Canada_Job_Market_Analysis.ipynb` — complete data cleaning, analysis, and visualization workflow
* `README.md` — project overview, methodology, findings, and limitations
