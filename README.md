<img width="1281" height="333" alt="Captura de pantalla 2026-05-20 123623" src="https://github.com/user-attachments/assets/6796b556-70b9-4dd1-ac7e-040c96148675" />
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

The palette desig draws inspiration from natural, earthy tones to create a grounded and professional visual aesthetic.

***Base & Background***
- The background uses a muted sage green (#BDC581).
- Text is rendered in near-black (#1A1A1A) for strong readability and contrast.

***Primary Greens:***
The core data colors range across a rich spectrum of greens, from deep forest (#2F3E1F) and dark olive (#344E41) to mid-range moss (#6B8E23) and sage (#8A9A5B).

***Cool Accents:***
A set of muted steel blues (#3D5A80, #577590, #2C3E50) provides contrast and visual balance, preventing the palette from feeling monotonous.

***Warm Neutrals & Earth Tones:***
Warm browns and tans (#BC6C25, #D4A373, #7F5539, #A98467) add warmth and depth. The burnt orange-brown (#BC6C25) also serves as the table accent, drawing attention to key data points.

***Neutral Grays:***
Grays (#6C757D, #495057) serve as supporting tones for secondary information, ensuring a clean hierarchy without competing with the main colors.

### Tabs

The information was show in sixs diferent tabs, to represent sixs different views of the information.

<img width="1901" height="749" alt="Captura de pantalla 2026-05-20 130841" src="https://github.com/user-attachments/assets/d54422b7-9adf-496d-a2e6-b91a2b05ff97" />

#### 1. Global View

This section features a map that updates dynamically as filters are modified. The available filters allow the user to select by Category (Cereals / Fibers / Fruits / Legumes / Oilseeds / Vegetables), Product, or Year (ranging from 1961 to 2024), with the option to select multiple values per filter. As the filters are adjusted, the map rescales the circle size for each country proportionally to its production volume. Additionally, a metric card highlights the country with the highest production for the current filter selection.

#### 2. Temporal Evolution

The Temporal Evolution section contains 3 dynamic charts displaying: 1) the overall production index per year, 2) the production index per year for the top five countries, and 3) the production index per year for the top products. It also includes 3 filters allowing the user to select by Country, Category, and Product. This section provides a general overview of the production trends over time, while the filters offer additional flexibility to narrow down or compare specific data points.

#### 3. Categories

This tab displays the contribution of each category to the total production of the region, allowing the user to understand which agricultural sectors, such as Cereals, Fruits, Vegetables, Legumes, Oilseeds, or Fibers, carry the most weight in the region overall output, and which Country leads in each Categorie. The available filters allow the user to adjust the country under analysis as well as the year.

#### 4. Country Comparison

The Country Comparison tab displays the top and bottom five countries by production, along with a general ranking overview. Users can adjust the Category filter to identify which countries contribute the most and the least to overall production, as well as define the time range for the analysis.

This tab is particularly useful for benchmarking countries against each other, spotting consistent top performers, and identifying underperforming nations across different agricultural categories and time periods.

#### 5. Explorer

This section offers greater flexibility to the user, providing the opportunity to interact with filters across all available variables. It features two visuals: the first is a detailed table displaying country, category, product, year, and production values, allowing for a precise and structured review of the data. The second is a more visual representation, making it easier to compare production levels across countries 
at a glance.

#### 6. Insights

The final tab features a line chart showing the average production index over time, alongside a horizontal bar chart ranking countries by their average production index, making it straightforward to compare relative performance across nations. Key metric cards highlight the leading country and its category, the top product, the fastest-growing country, as well as the bottom-performing country, category, and 
product with the lowest production per capita — offering a comprehensive summary of both extremes in a single view.

---

# Key Insights

1. Brazil has historically led production in the region.
2. 1971 recorded the highest production index, with Brazil as the leading country and Ramie as the standout product.
3. 40.61% of the region's total production corresponded to the Fibers category.
4. Guyana is the country with the lowest production in the region.

---

# Author

**Isabella Sierra Useche**

Bioengineering interested in:
- Data Analytics
- Artificial Intelligence
- Agro Security
- Environmental and Biological Data Science

---
