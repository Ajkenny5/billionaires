# ALL BILLIONAIRES 1997–2023
### Introduction

In an age where wealth distribution and billionaire trends are closely scrutinized, data storytelling becomes essential. This Power BI project explores the global billionaire ecosystem — analyzing demographic patterns, net worth trends, industry breakdowns, and geographical distributions. Using a refined, multi-dashboard approach, this report breaks down the state of wealth leadership from 1997 to 2023.

### Tools Used
- Microsoft Excel (for data cleaning and transformation)
- Microsoft Power BI (for dashboard design, DAX measures, and visuals)

### Data Source
[Download Here](https://drive.google.com/file/d/1BOJEn9bf9yLRoAL867bldMY42JeCq_FG/view)

### Data Cleaning and Data Preparation
- Over 30,000 records from 1997 to 2023.
- Well-structured with consistent column types and naming.
- The blank rows on the Rank column were filled manually for each year.
- The alphabet “B” on the net worth column was removed and each was multiplied by 1,000,000,000 (a billion)
- The cleaned name column used as the full name column, while the full name column was dropped.
- The birth date column was dropped, on the age column the blank rows and age zero (0) rows were replaced with the average age for each year.
- Blank rows on the gender column were replaced with the mode (Male).
- All other blank were replaced with the placeholder (NA).
- The organization name, position in organization and position columns were dropped due to high number of blank rows.

### Data Modelling
After ensuring my data’s accuracy and consistency, I began the process of creating a data model for my table by structuring the dataset to 5 different tables. I first establish my data table which is “Fact table” then started creating relationships between tables. For this project, I used “one to many” relationship.

### DAX Function
With the table relationships established, I utilized some DAX functions to analyze the dataset. I started by creating basic KPIs such as Total net_worth, Average net_worth, Number of Billionaire, etc, which would help in creating more advanced metrics later on. Some DAX functions I used the most are:

- Aggregate Function (SUM, COUNT, DISTINCTCOUNT & AVERAGE): This formula combines multiple values into a single value
- Calculate: Acts as an overriding filter to give you a new filter context.
- Date Function (DateAdd): This date function is very helpful in establishing previous year calculation.

![model](https://github.com/user-attachments/assets/b57ffe7a-633d-40b2-be3d-906e2a483f67)

### Dashboard Structure & Visual Highlights
Demographics

- Average Age: 66 years (vs. 65 last year)
- Billionaire age distribution peaks between 55–74
- Self-Made: 53.58%, Non Self-Made: 46.42%
- Gender: 89.15% Male, 10.85% Female
- Billionaires under 40: 63 for year 2023, down 17.11% for past year
- Wealth Status: Self-Made: 9.76K, Increased: 8.99K, Inherited: 7.68K, while other wealth status were below 5.00K.
- Yearly Trend of Billionaires: Increase in billionaires from the year 2010–2020.
- Total Billionaires: 2,640 (1.05% lower than the past year)
- An all-pages level Slicer “Gender, months and years” were used on this dashboard.

![D 1](https://github.com/user-attachments/assets/ede1a5df-d38e-4771-bae2-0d2d46a22dfe)



![Slicers](https://github.com/user-attachments/assets/1b982b65-0c3e-428f-881b-f8b717532a35)


Net Worth Trends & Individual Rankings:

- Total Net Worth: $12.21T (3.93% lower than past year (PY))
- Average Net Worth: $4.62B (2.91% lower than PY)
- Top Billionaires: Elon Musk for year 2022, Bernard Arnault year 2023, Jeff Bezos year 2019,2020,2021.
- Steady net worth growth trend post-2010
- Highest Net Worth: 211.00B (3.65% lower than PY)
- Average Net Worth vs Age Analysis: It displays a positive correlation, which means as the age increases, their average net worth increases.
- This dashboard can be filtered by a page-level Slicer “Full Name”.

![D2](https://github.com/user-attachments/assets/b315b68a-331e-498b-9c90-c925deef1642)


Top Industries and Business Domains:

- Popular sectors: Manufacturing, Technology, Finance, Real Estate
- Top Business by Avg Net Worth: Politics $12.5B, Luxury Goods $12.1B, and Biotech $9.7B.
- Top counties of citizenship by number of billionaires and average net worth: It show United States and China with 1,183 and 992 respectively. Despite China having high number of billionaires, they are the second lowest country of citizenship by average net worth.
- Countries of Citizenship: With a total of 70 countries in the current year (2023), it was 1.45% higher than the previous year.
- Countries of Residence: With a total of 79 countries of residence in the current year (2023), it was 6.76% higher than the previous year.
- Cities of Residence: With a total of 764 cities in the current year (2023), it was 0.13% lower than the previous year.

  
![D3](https://github.com/user-attachments/assets/e97355d9-b834-470e-86c4-3c11f9decb2f)


Geographical Analysis:
Country-Level Insights:

- The United States stands out as the global hub of billionaire wealth, both in terms of total net worth and number of individuals.

- China and Germany follow, with substantial billionaire populations, reflecting their growing global economic influence.

City-Level Observations:

- Cities such as New York, San Francisco, London, Hong Kong, and Beijing appear as high-density billionaire hubs.

- These cities serve as global financial centers, often linked with tech, finance, real estate, and luxury sectors — industries that dominate billionaire wealth.

- This dashboard can be filtered by a visual-level Slicer “Wealth status”.


![D4](https://github.com/user-attachments/assets/81eb9ad6-e2b3-4904-bbce-6d164454e672)


### Conclusion

The analysis of global billionaires from 1997 to 2023 reveals significant insights into the distribution, growth, and dynamics of extreme wealth worldwide. Over the years, the number of billionaires has increased substantially, although 2023 shows a slight decline in both count and cumulative net worth. The average age of billionaires remains steady at around 66, with a noticeable concentration in the 55–74 age range.

A dominant share of billionaires are self-made, yet that proportion has slightly decreased from the previous year. The gender imbalance is still stark, with females representing only 10.85% of all billionaires.

Business sectors like technology, finance, and manufacturing remain the most popular and lucrative, while countries such as the United States, China, and India dominate both in billionaire count and cumulative net worth.

Overall, the dashboard highlights key global wealth patterns, demographic shifts, and the influence of industries and geographies on wealth accumulation.




