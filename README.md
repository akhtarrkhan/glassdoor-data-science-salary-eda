# Glassdoor Data Science Salary EDA

## Project Overview

This project analyzes Glassdoor job posting data for data-related roles. The goal was to clean raw job posting data, engineer useful features, and explore salary patterns across job titles, locations, seniority levels, industries, company ratings, and technical skills.

This project helped me practise real-world data cleaning, salary parsing, feature engineering, and exploratory data analysis using Python.

## Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

The dataset contains Glassdoor job postings with fields such as:

- Job Title
- Salary Estimate
- Job Description
- Company Name
- Location
- Rating
- Industry
- Sector
- Revenue
- Competitors

The raw dataset was cleaned and transformed into `salary_data_cleaned.csv`.

## Key Cleaning Steps

- Removed records with missing salary estimates
- Parsed salary ranges into minimum, maximum, and average salary
- Created flags for hourly and employer-provided salary estimates
- Cleaned company names by removing rating text
- Extracted job state from location
- Created company age feature
- Created skill indicator columns for Python, R, Spark, AWS, Excel, and SQL

## EDA Performed

- Salary distribution analysis
- Company rating distribution
- Company age analysis
- Job description length analysis
- Correlation analysis between numeric variables
- Salary comparison by:
  - Job title
  - Seniority
  - Location
  - Industry
  - Sector
  - Revenue
  - Technical skills

## Key Insights

- Data Scientist, Data Engineer, Analyst, Machine Learning Engineer, Manager roles were grouped into simplified job categories.
- Seniority level was extracted from job titles to compare salary differences.
- Python, Spark, AWS, Excel, SQL, and R were converted into binary skill indicators.
- Pivot tables were used to compare average salary across job type, seniority, sector, revenue, and technical skills.

## Files in This Repository

| File | Description |
|---|---|
| `Cleaning_Jobs_Data.ipynb` | Cleans raw Glassdoor job posting data |
| `EDA_Jobs_Data.ipynb` | Performs exploratory data analysis |
| `data/glassdoor_jobs.csv` | Raw dataset |
| `data/salary_data_cleaned.csv` | Cleaned dataset used for EDA |
