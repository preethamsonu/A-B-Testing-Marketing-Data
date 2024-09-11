# A/B Testing of Ad Performance on Conversion Rates: A Data-Driven Approach
## 1. Introduction
In this project, we conducted A/B testing using a dataset from Kaggle, aiming to analyze the impact of a targeted advertisement on conversion rates compared to a public service announcement (PSA). The dataset provided insights into ad display patterns and their relationship to conversion success, allowing us to apply statistical hypothesis testing techniques. This report outlines our analysis, including univariate and bivariate analysis, and the statistical methods used to validate the findings.

## 2. Objective
The goal was to assess the effectiveness of repeated targeted ads in driving conversion rates compared to general public service announcements. Specifically, we aimed to:

Investigate which days and hours had the highest conversion rates.
Analyze the effect of repeated ad exposure on conversion success.
Validate these findings through appropriate statistical tests, such as the Mann-Whitney U test.
## 3. Dataset Overview
The dataset consisted of several variables:

Day of the week: The day ads were displayed.
Hour of the day: The time when ads were shown.
Total ads are shown: The number of ads displayed to each prospect.
Conversion status: Whether the prospect converted or not.
## 4. Exploratory Data Analysis
### 4.1 Univariate Analysis
We started by analyzing each variable individually:

Conversion by Day: The analysis revealed that the majority of conversions occurred on Monday, accounting for 3.2% of total conversions.
Conversion by Hour: Conversions peaked at 4 PM, indicating that ad exposure during this hour was particularly effective.
### 4.2 Bivariate Analysis
Next, we explored the relationship between ad exposure and conversion status:

Effect of Repeated Targeting: Our analysis suggested that repeated targeting significantly contributed to higher conversion rates. Prospects exposed to ads multiple times were more likely to convert than those shown fewer ads.
Median Ad Exposure: A box plot analysis showed that the median number of ads seen by prospects differed between converters and non-converters, with converters generally exposed to more ads.
## 5. Statistical Hypothesis Testing
### 5.1 Normality and Equality Testing
We conducted normality and equality tests on the data to determine the appropriate statistical methods for comparing groups. The results indicated that the data did not follow a normal distribution, making parametric tests like the T-test unsuitable.

### 5.2 Mann-Whitney U Test
Given the non-normal distribution, we used the Mann-Whitney U test to compare the distribution of total ads shown between converters and non-converters:

Null Hypothesis (H₀): There is no difference in the distribution of ads seen between converters and non-converters.
Alternative Hypothesis (H₁): There is a significant difference in the distribution of ads seen between converters and non-converters.
The Mann-Whitney U test results confirmed a significant difference, with prospects who converted having seen a higher median number of ads than those who didn’t.

## 6. Results and Insights
The key findings from this analysis are:

Most conversions occurred on Monday (3.2%).
The highest conversion rate was at 4 PM.
Repeated targeting led to an increased likelihood of conversion.
The median number of ads seen played a crucial role in determining whether a prospect converted.
## 7. Conclusion
The analysis showed that targeted ads, especially when shown multiple times, were more effective in driving conversions. Monday and 4 PM were identified as optimal times for displaying ads. The use of the Mann-Whitney U test provided robust statistical validation for these findings, confirming the significant impact of repeated ad exposure on conversion success.

Future research could focus on refining the targeting strategy based on ad timing and exploring additional factors influencing conversions.
