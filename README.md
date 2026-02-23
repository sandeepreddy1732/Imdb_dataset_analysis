


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
   imdbmovies_etl.ipynb
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

## Project Objective

This project demonstrates:

- Practical ETL workflow implementation  
- Business-rule-driven data transformation  
- Data validation and cleaning techniques  
- Analytical insights generation  
- End-to-end pipeline from raw dataset to database-ready format  
