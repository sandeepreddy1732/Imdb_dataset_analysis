


# IMDB Movie Dataset – ETL & Exploratory Data Analysis

## Problem Statement

The raw IMDB movie dataset contains inconsistencies, missing values, duplicate records, and unstructured fields that make it unsuitable for direct business reporting and dashboard development.

The objective of this project is to:

- Build a structured **ETL pipeline (Extract, Transform, Load)**
- Apply defined **business rules and validation logic**
- Clean and standardize the dataset
- Generate analytical insights for reporting
- Prepare a **database-ready cleaned dataset**

This project simulates a real-world data engineering workflow from raw data ingestion to analytics-ready output.

---

## Project Overview

This project performs:

- **Extract** → Load raw IMDB dataset  
- **Transform** → Clean, validate, standardize, and apply business logic  
- **Load** → Export cleaned dataset for relational database integration  
- **EDA** → Perform exploratory analysis and generate insights  

The final output is a structured dataset suitable for analytics and BI dashboards.

---

## Repository Contents

- [IMDB Movie Business Rules and dashboard_problems statements.txt](IMDB%20Movie%20Business%20Rules%20and%20dashboard_problems%20statements.txt): Business rules and problem statements for the dashboard.
- [imdb_ddl.sql](imdb_ddl.sql): DDL for loading the cleaned dataset into a relational database.
- [imdb_movies.csv](imdb_movies.csv): Original raw dataset (CSV).
- [imdb_movies_cleaned.csv](imdb_movies_cleaned.csv): Cleaned and preprocessed dataset exported from the notebook.
- [PROJECT_P1_IMDB_DATA_ANALYSIS.ipynb](PROJECT_P1_IMDB_DATA_ANALYSIS.ipynb): Main Jupyter notebook performing ETL and analysis.

---

## Steps Followed

 ## Data Cleaning (Python)

- Removed duplicate movie records based on **title and release year**
- Generated missing **movie IDs**
- Corrected invalid values in **ratings, budget, and gross**
- Replaced missing **director and actor names** with `"Unknown"`
- Filled missing **release years** using the **median value**

 ## Data Loading (MySQL)

- Connected Python to MySQL using **SQLAlchemy**
- Created a cleaned `movies` table
- Loaded the transformed dataset into MySQL database

 ## SQL Analysis

- Identified **top-grossing movies by year**
- Calculated **average rating by genre**
- Found **top directors based on average ratings**
- Analyzed **budget vs gross revenue relationship**
- Determined the **most profitable movie genre**

 ## Data Visualization

- Created **bar charts, line charts, and scatter plots** using Matplotlib
- Built simple dashboards to present key business insights

 ## Tech Stack

- Python 3.8+
- Jupyter Notebook
- pandas
- matplotlib
- sqlalchemy
- SQL (DDL for relational loading)

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
  
## Project Outcome

- Implemented structured ETL workflow  
- Applied real-world data validation logic  
- Generated business-driven insights  
- Prepared analytics-ready dataset  
