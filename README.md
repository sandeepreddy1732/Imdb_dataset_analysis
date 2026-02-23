


# IMDB Movie Dataset – ETL & Exploratory Data Analysis

## Overview

This project performs **ETL (Extract, Transform, Load)** and **Exploratory Data Analysis (EDA)** on an IMDB movie dataset using Python and Jupyter Notebook.

The notebook processes raw movie data, applies business rules, cleans inconsistencies, and generates analytical insights that can be used for reporting and dashboard development.

The final output is a cleaned dataset ready for database integration and business analysis.

---
## Repository Contents

- [IMDB Movie Business Rules and dashboard_problems statements.txt](IMDB%20Movie%20Business%20Rules%20and%20dashboard_problems%20statements.txt): Business rules and problem statements for the dashboard.
- [imdb_ddl.sql](imdb_ddl.sql): DDL for loading the cleaned dataset into a relational database.
- [imdb_movies.csv](imdb_movies.csv): Original raw dataset (CSV).
- [imdb_movies_cleaned.csv](imdb_movies_cleaned.csv): Cleaned and preprocessed dataset exported from the notebook.
- [imdbmovies_etl.ipynb](PROJECT_P1_IMDB_DATA_ANALYSIS.ipynb): Main Jupyter notebook performing ETL and analysis.

---

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - pandas
  - matplotlib
  - sqlalchemy

---

## Setup Instructions

Create a virtual environment:

```bash
python -m venv .venv
.\.venv\Scripts\activate
```

Install required packages:

```bash
pip install pandas matplotlib sqlalchemy jupyter
```

---

## How to Run the Project

1. Open the notebook:
   ```bash
   PROJECT_P1_IMDB_DATA_ANALYSIS.ipynb
   ```
   
2. Run all cells sequentially to:
   - Load raw data
   - Clean and transform the dataset
   - Apply business rules
   - Generate visualizations

---

## ETL Process Highlights

### Data Cleaning
- Handling missing values  
- Removing duplicates  
- Standardizing column names  
- Parsing date columns  
- Normalizing numeric fields  

### Business Rule Implementation
- Applying validation logic  
- Deriving calculated fields  
- Aggregations for analytics  
- Filtering and transformation as per defined rules  

### Data Visualization
- Movie release trends  
- Genre analysis  
- Rating distribution  
- Revenue analysis  

---

### Dashboard Modules & Analysis

**Dashboard 1: Revenue Analysis**

<img width="571" height="489" alt="image" src="https://raw.githubusercontent.com/sandeepreddy1732/Imdb_dataset_analysis/main/Reports/1.%20Top%2010%20Highest%20Grossing%20Movies%20by%20Year%20Result.png" />

- Identify the Top 10 highest-grossing movies each year
- Analyze year-over-year revenue trends
- Compare gross revenue performance across different years

**Dashboard 2: Genre Performance Insights**

<img width="580" height="455" alt="image" src="https://raw.githubusercontent.com/sandeepreddy1732/Imdb_dataset_analysis/main/Reports/2.%20Average%20Rating%20by%20Genre%20Result.png" />

- Evaluate average rating distribution across genres
- Analyze the total number of movies released per genre
- Compare profitability across different genres
  
**Dashboard 3: Director Performance Analysis**

<img width="585" height="455" alt="image" src="https://raw.githubusercontent.com/sandeepreddy1732/Imdb_dataset_analysis/main/Reports/3.%20Top%205%20Directors%20by%20Average%20Rating%20Result.png" />

- Identify the Top 5 directors based on average movie ratings
- Analyze the number of movies directed by each director
- Compare director performance based on rating metrics

**Dashboard 4: Budget & Profitability Analysis**

<img width="571" height="455" alt="image" src="https://raw.githubusercontent.com/sandeepreddy1732/Imdb_dataset_analysis/main/Reports/4.%20Budget%20vs%20Gross%20Correlation%20Result.png" />

- Examine the correlation between budget and gross revenue
- Identify the most profitable genre (Gross Revenue − Budget)
- Analyze overall profit trends across movies

**Dashboard 5: Most Profitable Genre Deep Dive**

<img width="589" height="455" alt="image" src="https://raw.githubusercontent.com/sandeepreddy1732/Imdb_dataset_analysis/main/Reports/5.%20Most%20Profitable%20Genre%20Result.png" />

- Perform in-depth analysis of genre profitability
- Evaluate profit margins across genres
- Compare genre performance trends over time
  
## Project Objective

This project demonstrates:

- Practical ETL workflow implementation  
- Business-rule-driven data transformation  
- Data validation and cleaning techniques  
- Analytical insights generation  
- End-to-end pipeline from raw dataset to database-ready format  
