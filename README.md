# Supply-Chain-Strategic
Product Placement

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Recommendations](#recommendations)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis-eda)
- [Data Analysis](#data-analysis)
- [Vizualizations](#visualizations)
- [Key Findings and Recommendations](#key-findings)
- [Limitations and References](#limitations)
- [References](#references)
- [Conclusion](#conclusion)

## Project Overview

This data analysis project aims to provide insights into employment trends across various industries in California from 2014 to 2024. By analyzing employment data, we seek to uncover trends, identify regional patterns, assess the impact of seasonality, and highlight industries experiencing significant growth or decline. Our findings are intended to inform workforce development initiatives and policy recommendations.

#### ![Employment Growth (Yr/Yr)](https://github.com/JoseAGonzalezR/CES/blob/main/Employment%20Growth.png)

## Data Sources

-	Current Employment Statistics Data: The primary dataset used in this analysis is the "ces_2014-2024_monthly_2024419.csv," which contains monthly employment data provided by the California Employment Development Department. This dataset includes industry-specific employment figures, seasonally adjusted metrics, and region-specific data for comprehensive insights.

## Tools

- Excel - Data Cleaning
- MySQL Server - Data Storage and Quering
- Python - Pandas
- Tableau - Data Visualization and Dashboard Creation

## Data Cleaning/Preparation

In the initial data preparation phase, I performed several steps to ensure accuracy and consistency:
1. Data loading and inspection: loaded data into MySQL and Tableau for seamless analysis.
2. Data Cleaning: Addressed missing values, filtered out not relevant rows, and standardized date formats
3. Column Creation: Added columns for California State location, and relevant categories for enhanced filtering.

## Exploratory Data Analysis (EDA)

During EDA, I explored the data to address key questions, such as:
- Employment Trends Over Time: How has employment changed across industries over the years?
- Regional Patterns: What are the employment trends across different area types (e.g., metropolitan vs. non-metropolitan)?
- Seasonal Employment Patterns: How does seasonally adjusted employment compare to non-adjusted figures over time?
- Industry Growth: Which industries have experienced the highest growth or decline?

## Data Analysis

In the analysis phase, I utilized SQL queries and Python with Pandas for data manipulation and to derive insights. Here’s an example SQL query used:
```sql
SELECT Industry_Title, Year, AVG(Current_Employment) as Avg_Employment
FROM ces_data
WHERE State = 'California'
GROUP BY Industry_Title, Year
ORDER BY Avg_Employment DESC;
```
## Key Findings

Key findings from the analysis include:
1. Employment Growth: Several industries, particularly those in tech and healthcare, have shown consistent employment growth, while others faced declines.
3. Seasonality Impact: Seasonally adjusted employment data reveal that certain industries experience recurring fluctuations, likely tied to specific times of the year.
4. Top-Performing Regions: Metropolitan areas consistently report higher employment rates, though certain rural areas show rapid growth in specific industries.

## Conclusion
This analysis of California’s employment trends from 2014 to 2024 provides valuable insights into the dynamics of different industries, geographic regions, and seasonal patterns within the state. By examining historical data, there were identified key drivers and challenges affecting employment, highlighting the impacts of economic cycles, industry-specific developments, and regional variations.

The data reveals that California's employment landscape has generally trended upward over the past decade, though recent declines in 2024 may reflect emerging challenges, potentially driven by broader economic factors or industry-specific downturns. This analysis also shows that employment growth varied significantly across industries, with sectors like technology, healthcare, and construction seeing steady gains, while traditional sectors such as manufacturing faced more volatility.

## Recommendations

Based on these findings the following recommendations can help support sustained employment growth and stability in California:
#### 1. Targeted support for Declining Sectors:
  Implement policies or workforce development programs aimed at stabilizing industries showing reduced growth, such as manufacturing.
#### 2.	Investment in High-Growth Industries:
  Continue supporting industries with strong growth potential, particularly in tech and healthcare, to sustain California’s competitive edge.
#### 3.	Regional Development Programs:
  Encourage investment in rural and underserved areas to balance growth across the state and reduce dependency on major metropolitan regions.


## Limitations

This analysis is based on available data up to May 2024, which may limit the insights on recent trends and emerging issues. Additional data and future analyses could provide a more comprehensive understanding of the factors influencing employment in California.

## Visualizations

The visualizations include bar plots, heatmaps, and line charts to effectively illustrate employment trends, grwth rates, and seasonal patterns across California.

### [Click to see Dashboard](https://public.tableau.com/app/profile/jose.gonzalez.ramirez/viz/Current-Employment_CA/Dashboard1?publish=yes)

## References

- California Employment Development Department: Primary dataset source.
- U.S. Bureau of Labor Statistics: Comparative industry growth metrics.

## Final Thoughts

This project demonstrates the power of data analysis for uncovering actionable insights into employment trends. By tracking industry, regional, and seasonal trends, California can better anticipate and respond to economic shifts, ultimately supporting a resilient workforce and a thriving economy.

## [Go back to my Webpage](https://JoseAGonzalezR.github.io/Jose_AGonzalez.github.io/)
