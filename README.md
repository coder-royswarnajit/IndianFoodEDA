# Exploratory Data Analysis on Indian Food

## Overview

This project performs an **Exploratory Data Analysis (EDA)** on the `indian_food.csv` dataset to gain insights into Indian cuisine. The analysis focuses on dietary classifications, flavor profiles, preparation and cooking times, regional diversity, and commonly used ingredients across Indian dishes.

The objective is to understand patterns and trends in Indian food using statistical summaries and visualizations.

---

## Dataset

The dataset `indian_food.csv` contains information about various Indian dishes and includes the following columns:

* **name** – Name of the dish
* **ingredients** – List of ingredients used in the dish
* **diet** – Dietary classification (vegetarian or non-vegetarian)
* **prep_time** – Preparation time (in minutes)
* **cook_time** – Cooking time (in minutes)
* **flavor_profile** – Flavor profile (e.g., sweet, spicy, bitter, sour)
* **course** – Course of the meal (e.g., dessert, main course, snack, starter)
* **state** – Indian state associated with the dish
* **region** – Region of India associated with the dish

---

## Analysis Performed

### 1. Basic Data Exploration

* Displayed the first few rows of the dataset
* Inspected column names and data types
* Reviewed dataset structure using:

  * `data.head()`
  * `data.columns`
  * `data.info()`

### 2. Frequency Distribution of Categorical Variables

* Analyzed the distribution of unique values for:

  * `diet`
  * `flavor_profile`
  * `course`
  * `state`
  * `region`

### 3. Handling Missing Values

* Identified placeholder values (`-1`) and missing entries
* Replaced invalid values with `numpy.nan` for proper analysis

### 4. Preparation and Cooking Time Analysis

* Grouped dishes by:

  * `diet`
  * `course`
* Computed statistical measures:

  * Mean
  * Minimum
  * Maximum
  * Standard deviation
* Applied to both `prep_time` and `cook_time`

### 5. Top Ingredients Analysis

* Parsed the `ingredients` column
* Extracted individual ingredients
* Counted and ranked the most frequently used ingredients

### 6. Distribution of Diet Types

* Visualized the proportion of vegetarian vs. non-vegetarian dishes
* Used an interactive **Plotly pie chart**

### 7. Cooking and Preparation Time Extremes

* Identified:

  * Top 10 dishes with the shortest times
  * Top 10 dishes with the longest times
* Visualized results using **Plotly bar charts**

### 8. Time Distribution Analysis

* Plotted histograms for:

  * `prep_time`
  * `cook_time`
* Observed overall distribution and skewness

### 9. Diet vs. Flavor Profile Relationship

* Created a cross-tabulation between:

  * `diet`
  * `flavor_profile`
* Visualized using a **Plotly grouped bar chart**

### 10. Ingredient Word Cloud

* Generated a word cloud to visually highlight the most common ingredients used in Indian cuisine

---

## Libraries Used

* **pandas** – Data manipulation and analysis
* **numpy** – Numerical computations
* **matplotlib.pyplot** – Static visualizations
* **seaborn** – Statistical data visualization
* **plotly.express** – Interactive charts
* **wordcloud** – Ingredient frequency visualization

---

## How to Run the Project

1. Open the Jupyter Notebook or Google Colab notebook.
2. Upload the `indian_food.csv` dataset.
3. Install required libraries (if not already available).
4. Run all cells sequentially to reproduce the analysis and visualizations.

---

## Conclusion

This EDA provides a comprehensive overview of Indian cuisine, highlighting dietary trends, regional diversity, preparation practices, and ingredient usage. The insights gained can support further research, recommendation systems, or cultural food studies.

---
