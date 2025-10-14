🏠 London Borough House Prices (1998–2018)
📘 Overview

This project explores how housing prices have changed across London boroughs between 1998 and 2018. Using publicly available housing data, the analysis identifies which boroughs experienced the greatest increase in average house prices over two decades and visualizes the long-term growth trends.

📊 Objective

To answer the key question:

“Which London boroughs have seen the greatest increase in housing prices, on average, over the last two decades?”

🧠 Methodology

Data Cleaning & Preparation:

Filtered data by London_Borough, Year, and Average_Price.

Removed missing values and standardized column names.

Function Creation:

Defined a function create_price_ratio() to calculate the price ratio between 1998 and 2018 for each borough.

Growth Calculation:

Computed percentage growth using:

𝐺
𝑟
𝑜
𝑤
𝑡
ℎ
%
=
(
1
𝑅
𝑎
𝑡
𝑖
𝑜
−
1
)
×
100
Growth%=(
Ratio
1
	​

−1)×100

Visualization:

Used bar plots (matplotlib) to highlight the boroughs with the highest growth rates.

💹 Key Findings (Top 15 Boroughs by Growth)
Rank	Borough	Ratio_2018	Growth %
1	Hackney	0.161	519.8%
2	Waltham Forest	0.171	483.5%
3	Southwark	0.181	451.6%
4	Lewisham	0.184	444.8%
5	Westminster	0.187	435.3%
6	Newham	0.188	430.8%
7	City of London	0.189	430.3%
8	Haringey	0.195	413.5%
9	Kensington & Chelsea	0.197	408.2%
10	Lambeth	0.202	395.8%
11	Camden	0.203	393.4%
12	Barking & Dagenham	0.204	389.6%
13	Brent	0.204	389.5%
14	Islington	0.207	384.2%
15	Greenwich	0.210	376.4%
📈 Visualization

The bar chart below shows the percentage growth in average house prices from 1998 to 2018 for the top 15 boroughs.
The plot reveals that Hackney and Waltham Forest experienced the highest growth, with prices increasing more than fivefold over 20 years.

(Sample code snippet used for visualization):

ax = top15.sort_values('Growth_%', ascending=False).plot(
    kind='barh', 
    x='Borough', 
    y='Growth_%', 
    figsize=(10,6), 
    color='skyblue'
)
ax.set_title('House Price Growth (1998–2018) by London Borough', fontsize=14)
ax.set_xlabel('Growth Percentage (%)')
ax.set_ylabel('London Borough')
plt.show()

🧩 Interpretation & Insights

Boroughs in East and Southeast London (e.g., Hackney, Waltham Forest, Lewisham, Newham) show the strongest price surges, reflecting extensive regeneration and transport improvements.

Inner-city boroughs (Southwark, Lambeth, Islington, Camden) benefited from proximity to central London and urban redevelopment.

High-end areas (Westminster, Kensington & Chelsea) saw strong growth but less dramatic relative increases due to already high 1998 prices.

Overall, the center of affordability and growth shifted eastward, with once underdeveloped boroughs transforming into thriving urban communities.

🧰 Tools & Libraries

Python 3

Pandas

Matplotlib

Jupyter Notebook

📁 Files in Repository

london_house_prices.ipynb → Main analysis notebook

data/ → Cleaned dataset (if included)

README.md → Project summary and documentation

🏁 Conclusion

Between 1998 and 2018, Hackney led all London boroughs in housing price growth, reflecting large-scale regeneration, gentrification, and increasing desirability of East London. This trend marks a significant transformation in London’s housing market, both economically and socially.
