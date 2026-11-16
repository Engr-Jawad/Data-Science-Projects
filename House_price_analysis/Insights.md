# House Price Analysis — Key Insights and Findings

## 1. House area analysis

- **Average house area:** 1,601.12 sqft
- **Maximum house area:** 3,426 sqft
- **Minimum house area:** 1 sqft

**Insight:** The dataset contains houses with considerably different areas. The minimum area of 1 sqft is unusual and should be investigated as a possible data-quality issue.

## 2. Bedrooms analysis

- **Average number of bedrooms:** 3
- **Maximum number of bedrooms:** 8
- **Minimum number of bedrooms:** 1
- **Most common number of bedrooms:** 3

**Insight:** Three-bedroom houses are the most common in this dataset.

## 3. House age analysis

- **Average house age:** 30 years
- **Minimum house age:** 1 year
- **Maximum house age:** 60 years

**Insight:** The dataset includes both newly constructed and older houses.

## 4. House price analysis

- **Average house price:** PKR 7,793,422.13
- **Median house price:** PKR 7,312,805
- **Minimum house price:** PKR 700,000
- **Maximum house price:** PKR 15,632,108.50

**Insight:** House prices are right-skewed. The mean is higher than the median, which is consistent with some relatively expensive houses pulling the average upward.

## 5. Relationship between area and price

- **Correlation:** approximately +0.87 (as reported)

**Insight:** Area and house price have a very strong positive linear relationship in this dataset. Larger houses generally tend to have higher prices. Correlation does not, by itself, prove causation.

## 6. Bedrooms versus average house price

| Number of bedrooms | Average house price (PKR) |
|---:|---:|
| 2 | 6,000,124 |
| 3 | 7,369,145 |
| 4 | 8,927,647 |
| 5 | 10,797,887 |

**Insight:** The average house price increases across these bedroom categories. This association may also reflect differences in area, location, and other property characteristics.

## 7. Relationship between house age and price

**Insight:** The analysis indicates a strong negative relationship between house age and price. Older houses generally tend to have lower prices in this dataset. Check the exact correlation coefficient to quantify the strength of this relationship.

## 8. Location-based analysis

Findings from the analysis:

- Urban houses generally have higher prices.
- Rural houses generally have lower prices.
- Urban locations contain the largest number of houses: **4,167**.
- Suburban houses have a greater average area than urban and rural houses.
- Suburban locations are more frequent among the top 10 most expensive houses.

**Insight:** Location is associated with differences in house prices and house sizes. The fact that suburban houses are larger on average, and appear frequently among the 10 most expensive houses, is worth investigating further.

##  Overall conclusions

1. House area has a strong positive relationship with price.
2. House age has a strong negative relationship with price.
3. Average prices increase across the reported bedroom categories.
4. House prices are right-skewed.
5. Location is associated with differences in house prices and house sizes.
6. The top 10 most expensive houses include more suburban properties, according to the analysis.

#