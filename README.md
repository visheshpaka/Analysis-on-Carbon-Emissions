# Global CO2 Emissions Analysis

## Project Overview
This project focuses on analyzing global CO2 emissions data spanning from 1750 to 2021. It leverages a comprehensive dataset of CO2 emission sources, including Coal, Oil, Gas, Cement, Flaring, and Per Capita emissions, to uncover trends and insights. The primary objective is to preprocess the dataset, handle missing values through advanced imputation techniques, and create visualizations for better understanding and decision-making.

## Key Objectives
- Clean and preprocess a large dataset with over 63,000 rows and 232 countries.
- Handle missing values using advanced techniques like Iterative Imputer and compare with mean-based imputation.
- Generate insights into global and country-level CO2 emissions trends.
- Visualize the distribution and contributions of various emission sources over the years.
- Create an interactive dashboard showcasing analysis and findings.

---

## Dataset
### Characteristics
- **Data Source**: CO2 emission records for 232 countries from 1750 to 2021.
- **Columns**:
  - **Country**: Name of the country.
  - **Year**: Year of the record.
  - **Total**: Total CO2 emissions (metric tons).
  - **Coal, Oil, Gas, Cement, Flaring, Other**: Emission contributions by category.
  - **Per Capita**: Emissions per person.

### Dataset Summary
- **Original Rows**: 63,104
- **Filtered Rows**: 21,697 (after removing rows where `Total` emissions are zero).
- **Null Values**:
  - Significant missing values in some columns, such as "Other" (92.5%).

---

## Methodology
### Data Preprocessing
1. **Handling Missing Values**:
   - Removed rows with zero `Total` emissions to focus on meaningful records.
   - Dropped columns with excessive missing values (e.g., "Other").
   - Used **Iterative Imputer** for advanced imputation, preserving relationships between variables.
   - Compared results with mean-based imputation to evaluate accuracy.

2. **Data Cleaning**:
   - Ensured data integrity by recalculating the `Total` column post-imputation.
   - Added country information back to the cleaned dataset.

### Visualization
- Created interactive visualizations, including:
  - **Pie Chart**: Emission source contributions (Coal, Oil, Gas, Cement, etc.).
  - **Trends**: Time series of global and country-specific CO2 emissions.
  - **Comparative Analysis**: Emissions by source over time.

---

## Results and Insights
- **Global Trends**:
  - Significant growth in CO2 emissions from 1750 to 2021.
  - Coal and Oil remain the largest contributors to total emissions.
- **Data Imputation**:
  - Iterative Imputer provided more robust results compared to mean-based imputation.
  - Retained natural variance and relationships within the dataset.
- **Visualization Highlights**:
  - The interactive dashboard showcases the rise in emissions by source and country.
  - Visual representation of emission distribution aids in policy-making and awareness.

---

## Tools and Technologies
- **Python Libraries**:
  - `pandas` for data manipulation.
  - `fancyimpute` for advanced imputation.
  - `matplotlib` for static visualizations.
  - `Google Sites` for creating an interactive dashboard.
- **Google Colab**: Used for computation and data processing.

---

## How to Use
1. **Setup Environment**:
   - Install necessary Python libraries:
     ```bash
     pip install pandas fancyimpute matplotlib
     ```
2. **Preprocess Data**:
   - Use the provided script to clean and preprocess the dataset.
3. **Visualization**:
   - Generate static plots using the scripts.
   - Access the interactive dashboard at the link below.

---

## Visualization and Analysis Dashboard
Explore all the visualizations and analysis through this interactive dashboard:
[Global Emissions Dashboard](https://sites.google.com/view/globalemissions/home)

---

## Future Enhancements
- Integrate machine learning models to predict future CO2 emission trends.
- Incorporate additional datasets like energy consumption and population growth for deeper insights.
- Develop real-time dashboards for monitoring CO2 emissions globally.
