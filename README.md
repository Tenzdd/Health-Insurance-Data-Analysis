# Health Insurance Analysis

## Table Of Contents
-[Project Overview](#project-overview)

-[Exploratory Data Analysis](#exploratory-data-analysis)

-[Findings](#findings)

### Project Overview

This dashboard aims to provide insights into the sales(claimed insurance) of different health insurance providers, also, the diagnosis for which the insurance has been claimed , the cost incurred to the providers and the product name of the insurance and various other factors has been accounted / analyzed for a better understanding of each provider's performance.

![Screenshot 2024-05-10 145853](https://github.com/Tenzdd/Health-Insurance-Data-Analysis/assets/120646586/c9515af5-fe3c-467b-9a03-1ffe3057fac2)

![Screenshot 2024-05-10 145337](https://github.com/Tenzdd/Health-Insurance-Data-Analysis/assets/120646586/8602ab2f-46e1-4dd8-b8dd-60df65f1d290)

![Screenshot 2024-05-10 145824](https://github.com/Tenzdd/Health-Insurance-Data-Analysis/assets/120646586/6ecb06de-788c-463e-8327-04ea87c9bdc7)

![Screenshot 2024-05-10 145757](https://github.com/Tenzdd/Health-Insurance-Data-Analysis/assets/120646586/c547896f-26c0-4668-91d0-c4587d26c8a9)








### Data Source

Claims_Usecase :- Primary data set used for this project is "Claims_Usecase.xlsx".


### Tools

- Excel - Data Cleaning and structuring
- Power BI - Dashboard Creation


### Data Cleaning / Preparation

In the initial Data Preparation phase, following tasks were performed:
1.Data Load and inspection 
2.Data Formatting


### Exploratory Data Analysis

It involved exploring and answering questions such as :
- which provider has sold the most no of insurance products.
- diagnosis for with the most amount of insurance has been claimed.
- MOM change in the claim amount.

### Data Analysis

Some of the dax used for dashboard are : 

- Mom% = DIVIDE([Total Claim Cost],CALCULATE([Total Claim Cost],PREVIOUSMONTH('Calendar'[Date])))
- Top Clinical Benefits = RANKX(ALL('Dataset'[HMO Clinical Benefit Desc]),[Total Claim Cost],,DESC)
- Top Diagnosis by Claim cost = IF([Diagnosis Rank] <= 'Top Diagnosis'[Top Diagnosis Value],[Total Claim Cost])


### Findings

There is a significance difference in sales among all the health insurance providers from oct 2013 to sept 2014.
The top 3 Diagnosis for which the most sum of insurance claimed are respectively Respiratory, Musculoskeletal Diseases followed by Digestive Diseases.
The sales is not linear through the year and rather sudden dips and surge however overall the sales has increased by over 1.2 Million dollars when comparing data from the start date to the end date.

