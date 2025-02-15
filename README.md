# Project Background
The marketing agency involved in this analysis aims to maximize ROI for its clients' ad campaigns. In 2019, two separate advertising campaigns were conducted on Facebook and AdWords. 
This analysis was undertaken to determine which platform delivers better results in terms of key performance indicators, including ad clicks, conversions, and overall cost-effectiveness. 
By uncovering these insights, the agency can better allocate its budget and optimize future marketing strategies for its clients.

# Data Structure 
The dataset contains 365 records corresponding to each day in 2019. Key features include:
- **Date:** The date of data collection.
- **Facebook Ad Campaign:** Information on clicks, conversions, and ad costs for Facebook.
- **AdWords Ad Campaign:** Similar data for the AdWords platform.

Key tables in the dataset:
- Facebook Ad Campaign
- AdWords Ad Campaign

Before conducting the analysis, the dataset underwent quality checks to ensure completeness and consistency. 

# Executive Summary

## Overview of Findings
- **Facebook Ads outperform AdWords:** The average number of conversions from Facebook ads is significantly higher than that of AdWords, with a mean conversion rate of 11.74 compared to 5.98 for AdWords.
- **Conversion Frequency:** Facebook ads show more frequent high-conversion days, while AdWords experiences either low or moderate conversion rates, with notable gaps in conversion numbers.
- **Correlation between Clicks and Sales:** A strong positive correlation (0.87) was found between Facebook ad clicks and sales, indicating that more Facebook ad clicks directly translate into more sales. For AdWords, the correlation was moderate (0.45), suggesting that other factors influence its sales effectiveness.
- **Cost-Effectiveness (CPC Trends):** Advertising costs fluctuate over the year. Notably, May and November show the lowest cost-per-conversion, suggesting more cost-effective periods, while February experiences the highest CPC, warranting a review of ad strategy during that month.
- **Hypothesis Testing:** The hypothesis that Facebook ads generate more conversions than AdWords was strongly supported by statistical analysis, with a T-statistic of 32.88 and a p-value of 9.35e-134.
- **Predictive Modeling:** The linear regression model demonstrates strong predictive power for Facebook conversions, with an R2 score of 76.35%, helping businesses forecast future conversion outcomes based on ad clicks.

## Main Insights:
- **Facebook Ads Are Highly Effective:** With a strong correlation between clicks and conversions, businesses should consider increasing their investment in Facebook advertising to drive more sales.
- **AdWords Optimization Needed:** While AdWords contributes to conversions, its effectiveness is more limited. A deeper analysis of campaign strategies is recommended.
- **Budget Allocation:** To maximize ROI, allocate more budget to months with historically lower CPC values, like May and November, and optimize campaigns during periods of high CPC, such as February.
- **Weekday Focus:** Concentrate ad spend and efforts on Mondays and Tuesdays, consistently showing higher conversion rates.

# Insights Deep Dive

## Ad Clicks Analysis:
All histograms related to clicks and conversions show somewhat symmetrical distributions, indicating relatively even distribution of these metrics.

<img src="img\Campaign_Performance.png">

<img src="img\Campaign_Performance_Adwords.png">

## Conversion Rates:
- **Facebook:** Observed higher conversion days more frequently than AdWords, which showed a tendency for either low or moderate conversion rates.
- **AdWords:** No conversions were observed in the range of 10-15, indicating a review of strategies may be needed.

<img src="img\Daily_Conversions.png">

## Cost Effectiveness:
A strong positive correlation (0.87) between Facebook ad clicks and sales indicates that Facebook ads are highly effective in driving sales.
AdWords ads also positively correlate with sales, but with a moderate coefficient (0.45), suggesting other factors influence their effectiveness.

<img src="img\Clicks.png">

## Hypothesis Testing:
_Hypothesis: Advertising on Facebook will result in a greater number of conversions compared to AdWords._
- The mean conversion rate for Facebook (11.74) is significantly higher than AdWords (5.98).
- T-statistic: 32.88, p-value: 9.35e-134 — strong evidence supporting that Facebook generates more conversions than AdWords.

**Recommendation:** Reallocate more resources towards Facebook advertising to capitalize on its higher conversion rates.

## Predictive Modeling:
A linear regression model showed that Facebook ad clicks explain 76.35% of the variance in conversions. This predictive capability helps in planning and optimizing future campaigns.

<img src="img\Model.png">

## Trends (CTR and Conversion Rate):
- **Weekday Performance:** Conversions are consistent, but Mondays and Tuesdays show higher conversion rates, indicating increased user engagement at the beginning of the week.
  
    <img src="img\Weekly_Conversions.png">
- **Monthly Conversion Trends:** Fluctuations in conversion rates were observed in February, April, May, June, August, and November, possibly due to seasonal trends or changes in marketing strategies.
  
    <img src="img\Monthly_Conversions.png">
- **CPC Trends:** May and November show lower CPC values, suggesting periods of higher advertising effectiveness, while February sees higher CPCs.
  
    <img src="img\CPC.png">

# Recommendations
Based on the findings from this analysis, the following recommendations are provided for future ad campaigns:
1. **Reallocate Budget to Facebook Ads:** Prioritize Facebook campaigns based on superior conversion rates and A/B test different ad creatives for optimization.
2. **Optimize AdWords with A/B Testing:** Review and adjust AdWords strategies using A/B testing to address conversion gaps and improve performance.
3. **Utilize Predictive Insights:** Leverage regression model data to set realistic targets and optimize Facebook ad spend.
4. **Launch Campaigns on Mondays and Tuesdays:** Focus efforts on these weekdays when user engagement is highest for conversions.
5. **Adjust Budgets Based on CPC Trends:** Shift spending to lower-cost months like May and November to maximize cost-effectiveness.


# Tools and Technologies:

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
[![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?logo=matplotlib&logoColor=fff)](#)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)
[![Anaconda](https://img.shields.io/badge/Anaconda-44A833?logo=anaconda&logoColor=fff)](#)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
[![Uses LinearRegression](https://img.shields.io/badge/Uses-LinearRegression-green)](https://www.statsmodels.org/stable/generated/statsmodels.regression.linear_model.OLS.html)
[![Made with statsmodels](https://img.shields.io/badge/Made%20with-statsmodels-blue)](https://www.statsmodels.org/)
[![Uses seasonal_decompose](https://img.shields.io/badge/Uses-seasonal__decompose-blue)](https://www.statsmodels.org/stable/generated/statsmodels.tsa.seasonal.seasonal_decompose.html)
[![Uses coint](https://img.shields.io/badge/Uses-coint-green)](https://www.statsmodels.org/stable/generated/statsmodels.tsa.stattools.coint.html)
[![Powered by Seaborn](https://img.shields.io/badge/Powered%20by-Seaborn-orange)](https://seaborn.pydata.org/)