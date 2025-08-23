# Amazon Sales Analysis

This project demonstrates **data cleaning, filtering, and dashboard creation** for Amazon product sales data.
It is divided into two main phases:

1. **Data Cleaning & Export** (Python Notebook)
2. **Data Analysis & Dashboard** (Excel)

---

## 1) Data Cleaning & Export (Python Notebook)

**Step 1: Run the Notebook**

* Open the Jupyter Notebook provided.
* Run all cells to:

  * Clean the raw Amazon sales dataset (`amazon.csv`)
  * Remove duplicates, invalid values, and missing key data
  * Convert prices, discounts, ratings, and counts into numeric formats
  * Apply filtering (only products with rating ≥ 3 and reviews ≥ 50)

**Step 2: Export the Cleaned Dataset**

* The notebook will generate a file:

  ```
  cleaned_amazon_sales.csv
  ```
* This file will be used for Excel-based analysis.

---

## 2) Data Analysis & Dashboard (Excel)

**Step 1: Import Data**

* Open Excel → **Data → Get Data → From Text/CSV**
* Load `cleaned_amazon_sales.csv` into a new worksheet
* Convert the dataset into a **Table** (Ctrl + T) for structured analysis

---

**Step 2: Create PivotTables**

1. **Categories With Most Products**

   * Rows: `Category`
   * Values: `Product ID` (Count)

2. **Average Rating vs Rating Count per Category**

   * Rows: `Category`
   * Values: `Rating` (Average)
   * Values: `Rating Count` (Sum)

3. **Lowest vs Highest Price per Category**

   * Rows: `Category`
   * Values: `Actual Price` (Min, Max)

---

**Step 3: Create Charts for Dashboard**

On a new worksheet (Dashboard sheet):

1. **Bar Chart** → Categories with Most Products
2. **Bar + Line Combo Chart** → Avg Rating vs Rating Count per Category
3. **Line Chart** → Lowest vs Highest Price per Category

   * Add a **Slicer (Rating)** for interactive filtering

---

## 3) Final Deliverable: Excel Dashboard

Your dashboard now shows:

* Which categories have the **most products**
* How **average rating compares with rating count** across categories
* How **prices vary per category** (lowest vs highest)
* Interactive filtering using slicers

---

## Project Files

* `amazon.csv` → Original dataset
* `cleaned_amazon_sales.csv` → Cleaned and filtered dataset (output from Python)
* `Amazon_Dashboard.xlsx` → Excel Workbook file

---


**End Result**: A cleaned dataset ready for analysis + an interactive Excel dashboard with product/category insights.

---

**Dataset Source:** [Amazon Sales Dataset by Karkavelrajaj on Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)


