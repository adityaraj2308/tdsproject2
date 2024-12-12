# Dataset Analysis Report

## Insights from LLM

```markdown
# README.md

## Dataset Overview
This dataset comprises various metrics related to life satisfaction, economic factors, and social support across different countries and years. It includes measures such as the "Life Ladder" which represents subjective well-being, along with correlating factors like GDP per capita, social support, and perceptions of corruption.

## Summary Statistics
The dataset contains 2363 entries with various fields related to well-being metrics. Below is a summary of the key statistics:

| Statistic                       | Year          | Life Ladder  | Log GDP per capita | Social Support | Healthy Life Expectancy | Freedom to Make Life Choices | Generosity | Perceptions of Corruption | Positive Affect | Negative Affect | Cluster  |
|----------------------------------|---------------|--------------|---------------------|----------------|--------------------------|-----------------------------|------------|--------------------------|------------------|-----------------|----------|
| Count                           | 2363          | 2363         | 2335                | 2350           | 2300                     | 2327                        | 2282       | 2238                     | 2339             | 2347            | 2097     |
| Mean                            | 2014.76       | 5.48         | 9.40                | 0.81           | -                        | -                           | -          | 0.74                     | 0.65             | 0.27            | 0.49     |
| Standard Deviation              | 5.06          | 1.13         | 1.15                | 0.12           | -                        | -                           | -          | 0.18                     | 0.11             | 0.09            | 0.50     |
| Min                             | 2005          | 1.28         | 5.53                | 0.23           | -                        | -                           | -          | 0.04                     | 0.18             | 0.08            | 0.00     |
| 25th Percentile                 | 2011          | 4.65         | 8.51                | 0.74           | -                        | -                           | -          | 0.69                     | 0.57             | 0.21            | 0.00     |
| Median                          | 2015          | 5.45         | 9.50                | 0.83           | -                        | -                           | -          | 0.80                     | 0.66             | 0.26            | 0.00     |
| 75th Percentile                 | 2019          | 6.32         | 10.39               | 0.90           | -                        | -                           | -          | 0.87                     | 0.74             | 0.33            | 1.00     |
| Max                             | 2023          | 8.02         | 11.68               | 0.99           | -                        | -                           | -          | 0.98                     | 0.88             | 0.71            | 1.00     |

### Missing Values
The dataset has some missing values across various columns:

- **Log GDP per capita:** 28 missing values
- **Social support:** 13 missing values
- **Healthy life expectancy at birth:** 63 missing values
- **Freedom to make life choices:** 36 missing values
- **Generosity:** 81 missing values
- **Perceptions of corruption:** 125 missing values
- **Positive affect:** 24 missing values
- **Negative affect:** 16 missing values

## Analysis Steps
1. **Load the Dataset:** Import necessary libraries and load the dataset for analysis.
2. **Data Cleaning:** Address missing values appropriately, whether through imputation or removal.
3. **Exploratory Data Analysis (EDA):** Perform statistical analysis and visualize data distributions and relationships.
4. **Correlation Analysis:** Generate a correlation heatmap to understand relationships among various metrics.
5. **Clustering:** Apply KMeans clustering to group countries based on the features provided.
6. **Visualization:** Save visualizations as images (e.g., heatmap) and save clustered data to a CSV file.

## Key Findings
- There is a significant correlation between GDP per capita and the Life Ladder, suggesting that wealthier nations tend to report higher levels of life satisfaction.
- The analysis revealed clusters in the dataset, indicating different groups of countries sharing similar characteristics in terms of life satisfaction and economic metrics.
  
## Visualizations
- **Correlation Heatmap:** Displays the correlation coefficients among the different metrics in the dataset. 
  ![Correlation Heatmap](.png)
  
- **KMeans Clustering Output:** Clustering results that categorize countries into groups based on their metrics.
  - The clustered data can be accessed [here](./clustered_data.csv).

## Conclusion
This analysis provides valuable insights into the factors that influence happiness and satisfaction across various countries. The correlations identified can help policymakers focus on key areas affecting life satisfaction, while clustering offers a framework to analyze and compare countries systematically.

```


## Correlation Heatmap
![Correlation Heatmap](.png)

## KMeans Clustering
Clustered data saved as [clustered_data.csv](.\clustered_data.csv)