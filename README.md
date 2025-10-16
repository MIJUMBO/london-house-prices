# 🏠 London Borough House Prices (1998–2018)

## 📘 Overview
This project analyzes housing price changes across **London boroughs** from **1998 to 2018**, identifying which areas experienced the greatest increase in average house prices and exploring the factors behind this growth.

---

## 🎯 Objective
> **Which London boroughs have seen the greatest increase in housing prices, on average, over the last two decades?**

---

## 🧮 Methodology

1. **Data Cleaning & Preparation**
   - Filtered data by `London_Borough`, `Year`, and `Average_Price`.
   - Removed missing values and standardized column names.

2. **Function Creation**
   - Defined a function `create_price_ratio()` to calculate the price ratio between 1998 and 2018 for each borough.

3. **Growth Calculation**
   - Defined create_price_ratio by dividing [price_1998/price_2018] across each of London Borough.
   - Computed percentage growth using:  
     Growth\% = (1 / df_ratios['Ratio_2018'] - 1) * 100
     
 4. **Visualization**
   - Created horizontal bar charts to display the top 15 boroughs with the highest growth    
---

## 💹 Key Findings **

## Top 15 Boroughs by Growth (%)*

| Rank | Borough | Ratio_2018 | Growth % |
|:----:|:---------|:-----------|:----------|
| 1 | **Hackney** | 0.161 | **519.8%** |
| 2 | **Waltham Forest** | 0.171 | **483.5%** |
| 3 | **Southwark** | 0.181 | **451.6%** |
| 4 | **Lewisham** | 0.184 | **444.8%** |
| 5 | **Westminster** | 0.187 | **435.3%** |
| 6 | **Newham** | 0.188 | **430.8%** |
| 7 | **City of London** | 0.189 | **430.3%** |
| 8 | **Haringey** | 0.195 | **413.5%** |
| 9 | **Kensington & Chelsea** | 0.197 | **408.2%** |
| 10 | **Lambeth** | 0.202 | **395.8%** |
| 11 | **Camden** | 0.203 | **393.4%** |
| 12 | **Barking & Dagenham** | 0.204 | **389.6%** |
| 13 | **Brent** | 0.204 | **389.5%** |
| 14 | **Islington** | 0.207 | **384.2%** |
| 15 | **Greenwich** | 0.210 | **376.4%** |


## 📊 Average House Price Growth (1998–2018)
![House Price Growth](https://github.com/MIJUMBO/london-house-prices/blob/main/house_price_growth.png?raw=true)

---

## 🧠 Insights

1. East and Southeast London (Hackney, Waltham Forest, Lewisham, Newham) experienced the highest growth — driven by regeneration, improved transport, and affordability.

2. Inner-city boroughs (Southwark, Lambeth, Camden) also grew strongly due to urban redevelopment and proximity to central London.

3. Prime boroughs (Westminster, Kensington & Chelsea) still grew significantly, showing strong long-term demand.

4. Overall, London’s center of growth shifted eastward, transforming once lower-cost areas into vibrant communities.

---

##  Conclusion

Between 1998 and 2018, Hackney experienced the largest growth in average house prices (over 500%), reflecting regeneration,
gentrification, and transport improvements.This trend highlights the significant economic and social transformation across
East London over the past two decades.

## 🧰 Tools Used

Python 3

Pandas

Matplotlib

Jupyter Notebook


---

## 📁 Repository Contents

london-house-prices.ipynb → Main analysis notebook

data/ → Cleaned dataset (included)

README.md → Project summary and insights


---


