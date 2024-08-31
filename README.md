# Global Fertility Decline Analysis 
### Project Overview:
According to the record, The global Total Fertility Rate (TFR) has seen a significant decline, dropping from nearly 5 children per woman 70 years ago to 2.3 children today. This sharp decrease reflects profound changes in global demographic trends, and while it suggests progress in areas like family planning and economic development, it also introduces new uncertainties and challenges. 

This project explores the decline in fertility rates across 20 countries over a 40-year span (1984-2023). The countries are divided into two groups—those with the highest fertility rates and those with the lowest. The analysis aims to uncover the commonalities and differences between these groups and to analyze the relationship between fertility and key factors such as economic sectors, demographics, education, and health system.​

### Data Source
The dataset used in this analysis is sourced from the [World Bank Group](https://databank.worldbank.org/reports.aspx?source=2&series=SP.DYN.TFRT.IN&country=&_gl=1*1a5qzzn*_gcl_au*MTczNDYzNTAzLjE3MjM4MzUwNjM.#), covering 20 countries from 1984 to 2023, with a total of 8,000 entries. The countries are divided into two groups: the 10 countries with the highest fertility rates and the 10 with the lowest.

### Project Structure
This project is organized as follows:
- Dataset: High Fertility & Low Fertility Country dataset csv
- Descriptive Data: Metadata excel file
- Interactive Dashboard

### Key Findings
**High-Fertility Countries:​**
- Predominantly located in Africa.​
- Characterized by low GDP, low health expenditure, and low urbanization.​
- Over 75% population employed for agriculture.​
- Over the past 40 years, these countries have faced challenges such as corruption, political conflict, and widespread poverty.​
  
**Low-Fertility Countries:​**
- Mostly found in East Asia and Europe.​
- Display higher GDP, higher health expenditure, and higher urbanization.​
- Diverse Economy activities with emphasis on technology, finance, and manufacturing. ​
- Stable political environments with less corruption and no ongoing wars, excluding Ukraine due to ongoing conflicts.​
  
**Common Trends:​**
- Both groups show a decreasing trend in fertility rates over the 40-year period.​
- Despite the fertility decline, GDP has grown, and spending on health has increased in both groups.

### Model Evaluation:

- **Polynomial Regression**
- **LassoCV** (Best model for analyzing highest fertility rates, excluding unemployment feature due to missing data)
  - **Performance:**
    - Mean Absolute Error (MAE): 0.14
    - Mean Squared Error (MSE): 0.04
    - Root Mean Squared Error (RMSE): 0.20
    - R-squared: 0.94
- **RidgeCV** (Best model for analyzing lowest fertility rates combined, considering all 12 features)
  - **Performance:**
    - Mean Absolute Error (MAE): 0.09
    - Mean Squared Error (MSE): 0.01
    - Root Mean Squared Error (RMSE): 0.12
    - R-squared: 0.88


