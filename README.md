![alt text](image-1.png)
# GROSS PRODUCTION INDEX PER CAPITAL IN SOUTH AMERICA

This project analyzes the agricultural production index per capita in South America using data from the FAOSTAT database between 1961 and 2024. The dashboard was developed in Power BI to explore production trends, country comparisons, dominant agricultural categories in each country, and temporal evolution across the region.

The main objective of this project is to transform raw agricultural production data into an interactive analytical platform that helps understand the information.

---

# Dataset

**Source:** Food and Agriculture Organization (FAO) - FAOSTAT 

- FAOSTAT:  Indices of agricultural production 
            https://www.fao.org/faostat/es/#data/QI

---

# Tools Implemented

- Analytics platform - interactive dashboard: Power BI
- Programming Language for Data analysis: Python  3.13.13
- Excel

---

# Main Problems

1. Data cleaning (Dataset inconsistencies / Duplicate countries and regions / Non-optimal structure)
2. Identify the most suitable data visualization to display the desired information.
3. Tab organization and content layout.

---

# Step-by-Step / How to Replicate

## Retrieve Data

The data used comes from the Food and Agriculture Organization (FAO) dataset "FAOSTAT" (https://www.fao.org/faostat/es/#data/QI), under the "Production" section, where the option **Bulk Download → All Data** was selected. The download yielded 6 files: two containing Area Codes and Products, two containing Elements and Symbols, and the remaining two containing all the information — one with flags and one without. The file 
selected was the one containing all data without flags, resulting in a starting file size of 29,279 KB.

## Data Cleaning

For this project, this stage was carried out in Excel, where the objective was to take a raw text file and transform it into structured, usable information. The steps taken where ...

1. Convert text to columns.
2. Fix text encoding issues caused by special character symbols.
3. In decimal numbers, replace "." with ",".
4. Remove unnecessary columns (Area Code / Area Code (M49) / Product Code / Product Code (CPC) / Element Code / Unit / Y1964F).
5. Remove unnecessary rows in the countries section (Regions / Distinctive groupings).
6. Add a product category column.
7. Split the data by region (Africa / East Asia & Pacific / South Asia / Central Asia / Middle East & Western Asia / Eastern Europe & Central Asia /    Western & Northern Europe / North & Central America / South America).

## Import Data to Power BI

1. Load data from an excel file.
2. Transform South America data.
3. Promote first row to header.
4. Unpivot other columns.
5. Rename column titles (Year / Index).
6. Apply data adjustments.

## Desing Dashboard
 
### Color Palette

### Tabs