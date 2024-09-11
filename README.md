A/B Testing of Ad Performance on Conversion Rates: A Data-Driven Approach
1. Introduction
In this project, we applied A/B testing techniques to analyze the impact of an advertisement displayed to a test group against a general public service announcement (PSA) on conversion rates. The dataset, sourced from Kaggle, provides real-world data on ad displays and conversion outcomes, offering a valuable opportunity to explore the relationship between variables such as display time and conversion success. This report details our approach, including exploratory data analysis (EDA), hypothesis testing, and the conclusions drawn from the results.
2. Objective
The primary objective of this project was to determine whether the advertisement had a statistically significant effect on conversion rates compared to the general PSA. We aimed to:
•	Analyze ad display patterns (by day and hour) and their impact on conversion rates.
•	Use statistical methods to assess the relationship between ad exposure and conversion success.
•	Validate the results using hypothesis testing techniques such as the chi-squared test and Mann-Whitney U test.
3. Dataset Overview
The dataset contained several key variables:
•	Day of the week: The day when the ads were displayed.
•	Hour of the day: The specific time when the ads were shown.
•	Total ads shown: The number of ads displayed to prospects.
•	Conversion status: Whether the user converted (success) or not (failure).
The dataset included both categorical and continuous variables, making it well-suited for a variety of statistical techniques and visualizations.
4. Exploratory Data Analysis (EDA)
To begin, we explored the dataset to uncover patterns that could inform our A/B testing approach:
•	Ad Displays by Day: We analyzed which day of the week had the highest ad displays, identifying trends in user engagement across the week. The day with the most ad displays was visualized using a stacked bar chart, showing conversion rates for both the ad and PSA groups.
•	Ad Displays by Hour: Similarly, we investigated the hour of the day with the most ad displays, using a pie chart to compare ad exposure during peak hours versus non-peak hours. This analysis helped identify optimal times for ad placement.
•	Conversion Rates: We examined the relationship between total ads shown and conversion status. A box plot was created to visualize the distribution of conversions across different groups, providing insights into whether more ads led to higher conversions.
Key findings from the EDA revealed that ad displays were not uniformly distributed throughout the week or day, and certain times saw higher conversion rates, suggesting potential time-dependent effects.
5. Statistical Hypothesis Testing
5.1 Chi-Squared Test of Independence
We employed the chi-squared test to assess whether the conversion status (success/failure) was independent of the ad type (test group ad vs. PSA). This test allowed us to evaluate whether there was a significant relationship between these two categorical variables.
•	Null Hypothesis (H₀): Conversion status is independent of the ad type.
•	Alternative Hypothesis (H₁): Conversion status is dependent on the ad type.
The p-value from the chi-squared test was below the 0.05 significance level, indicating a statistically significant relationship between the ad type and conversion status. The test group ad was more effective in driving conversions than the PSA.
5.2 Mann-Whitney U Test
Next, we used the Mann-Whitney U test to compare the distribution of a continuous variable (total ads shown) between the two groups (test group and PSA). This non-parametric test helped us determine if there was a significant difference in conversion patterns between the two groups without assuming a normal distribution.
•	Null Hypothesis (H₀): The distributions of the two groups are the same.
•	Alternative Hypothesis (H₁): The distributions of the two groups are different.
The test results confirmed a significant difference in ad performance between the two groups, with the test group outperforming the PSA in terms of conversion rates.
6. Results and Insights
Our analysis produced the following key insights:
•	Time-Sensitive Ad Performance: Ads displayed during certain hours and days were more effective in driving conversions, suggesting that ad timing plays a critical role in engagement.
•	Significant Impact of Targeted Ads: The chi-squared test revealed that the targeted ad had a statistically significant impact on conversion rates compared to the PSA.
•	Distribution of Ad Exposure: The Mann-Whitney U test showed a clear difference in how the number of ads shown affected the two groups, further supporting the effectiveness of targeted advertising over general messaging.
7. Conclusion
The A/B testing results confirmed that the ad shown to the test group significantly outperformed the PSA in driving conversions. By leveraging insights from EDA and hypothesis testing, we were able to demonstrate the value of targeted advertising in increasing conversion rates.
This project highlights the importance of A/B testing as a tool for data-driven decision-making in marketing strategies. Future work could explore optimizing ad timing and further segmenting user groups to refine advertising efforts.
________________________________________
This structure ensures clarity and coherence, with each section building on the previous one to guide readers through the analysis and findings. Would you like to adjust or expand any sections of this report?
4o
You said:
The data set used in this is from kaggle link: https://www.kaggle.com/code/adhamtarek147/a-b-testing-analysis. These are some of the things that are found. You did Univariate Analysis, Bivariate Analysis and Satistical Tests and found out 1. Most conversions are done on Monday with 3.2% 2. Most conversions are done at 4 PM. 3. Repated targeting is helping in conversion rate 4. The median of total ads people saw makes difference in conversion status You performed Normality and Equality test and found out Mann-Whitney U test is more suitable than T-Test.
ChatGPT said:
ChatGPT
Memory updated
Here’s how I would incorporate these insights into the report:
________________________________________
A/B Testing of Ad Performance on Conversion Rates: A Data-Driven Approach
1. Introduction
In this project, we conducted A/B testing using a dataset from Kaggle, aiming to analyze the impact of a targeted advertisement on conversion rates compared to a public service announcement (PSA). The dataset provided insights into ad display patterns and their relationship to conversion success, allowing us to apply statistical hypothesis testing techniques. This report outlines our analysis, including univariate and bivariate analysis, and the statistical methods used to validate the findings.
2. Objective
The goal was to assess the effectiveness of repeated targeted ads in driving conversion rates compared to general public service announcements. Specifically, we aimed to:
•	Investigate which days and hours had the highest conversion rates.
•	Analyze the effect of repeated ad exposure on conversion success.
•	Validate these findings through appropriate statistical tests, such as the Mann-Whitney U test.
3. Dataset Overview
The dataset consisted of several variables:
•	Day of the week: The day ads were displayed.
•	Hour of the day: The time when ads were shown.
•	Total ads shown: The number of ads displayed to each prospect.
•	Conversion status: Whether the prospect converted or not.
4. Exploratory Data Analysis
4.1 Univariate Analysis
We started by analyzing each variable individually:
•	Conversion by Day: The analysis revealed that the majority of conversions occurred on Monday, accounting for 3.2% of total conversions.
•	Conversion by Hour: Conversions peaked at 4 PM, indicating that ad exposure during this hour was particularly effective.
4.2 Bivariate Analysis
Next, we explored the relationship between ad exposure and conversion status:
•	Effect of Repeated Targeting: Our analysis suggested that repeated targeting significantly contributed to higher conversion rates. Prospects exposed to ads multiple times were more likely to convert than those shown fewer ads.
•	Median Ad Exposure: A box plot analysis showed that the median number of ads seen by prospects differed between converters and non-converters, with converters generally exposed to more ads.
5. Statistical Hypothesis Testing
5.1 Normality and Equality Testing
We conducted normality and equality tests on the data to determine the appropriate statistical methods for comparing groups. The results indicated that the data did not follow a normal distribution, making parametric tests like the T-test unsuitable.
5.2 Mann-Whitney U Test
Given the non-normal distribution, we used the Mann-Whitney U test to compare the distribution of total ads shown between converters and non-converters:
•	Null Hypothesis (H₀): There is no difference in the distribution of ads seen between converters and non-converters.
•	Alternative Hypothesis (H₁): There is a significant difference in the distribution of ads seen between converters and non-converters.
The Mann-Whitney U test results confirmed a significant difference, with prospects who converted having seen a higher median number of ads than those who didn’t convert.
6. Results and Insights
The key findings from this analysis are:
1.	Most conversions occurred on Monday (3.2%).
2.	The highest conversion rate was at 4 PM.
3.	Repeated targeting led to an increased likelihood of conversion.
4.	The median number of ads seen played a crucial role in determining whether a prospect converted or not.
7. Conclusion
The analysis showed that targeted ads, especially when shown multiple times, were more effective in driving conversions. Monday and 4 PM were identified as optimal times for displaying ads. The use of the Mann-Whitney U test provided robust statistical validation for these findings, confirming the significant impact of repeated ad exposure on conversion success.
Future research could focus on refining the targeting strategy based on ad timing and exploring additional factors influencing conversions.

