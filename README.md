# TMDB Data Wrangling Project

## Project Overview
This project involves data wrangling techniques applied to the **TMDB (The Movie Database)** dataset. The aim is to clean, transform, and analyse movie-related data to extract useful insights, perform exploratory data analysis (EDA), and prepare the data for further analysis or machine learning tasks.

The dataset contains movie details, including release dates, budgets, revenues, ratings, genres, and more. The main steps in this project include:

- Data cleaning and handling missing values
- Data transformation and normalisation
- Feature engineering (e.g., extracting release years and categorising by decades)
- Exploratory data analysis (EDA) using visualisations
- Identifying trends and patterns in movie data

## Dataset
The dataset used in this project is from the **The Movie Database (TMDb)** and contains information about movies such as:
- **Movie title**
- **Release date**
- **Budget**
- **Revenue**
- **Genres**
- **Ratings**
- **Popularity**
- **Runtime**

### Data Source:
The data is available through the TMDb API or other pre-collected datasets that can be found on Kaggle or other repositories. It is assumed that this dataset has been pre-collected and stored in CSV format for use in the project.

## Key Project Steps
### 1. Data Import and Initial Inspection
The data was loaded using **Pandas** and initially inspected to identify any missing or erroneous values. The structure and basic statistics of the dataset were examined to guide further steps.

### 2. Data Cleaning
Several data cleaning tasks were performed, including:
- Handling missing values (either by imputation or removal).
- Removing duplicate rows.
- Correcting data types (e.g., converting columns to appropriate formats such as integers or floats).
  
### 3. Feature Engineering
- **Release Year Extraction**: The `release_date` column was used to extract the year of release and create a new `release_year` column.
- **Decade Classification**: Movies were grouped into decades based on their release year.
- **Revenue vs Budget Comparison**: A comparison was made between budget and revenue for various movies, highlighting the biggest flops and successes.

### 4. Exploratory Data Analysis (EDA)
Key visualisations were created to uncover patterns and trends in the dataset. Some of the EDA tasks included:
- Plotting the distribution of movie budgets and revenues.
- Comparing movie budgets vs revenue for the biggest flops and successes.
- Analysing the number of movies released by decade.
  
### 5. Data Transformation
The dataset was transformed into a long format for easier analysis using `pd.melt()` to compare budgets and revenues side by side for visualisation.

## Technologies Used
- **Python** (for scripting and data analysis)
- **Pandas** (for data manipulation)
- **Matplotlib/Seaborn** (for data visualisation)
- **NumPy** (for numerical operations)

## Installation
To run this project on your local machine, ensure that you have the required libraries installed:

```bash
pip install pandas numpy matplotlib seaborn

