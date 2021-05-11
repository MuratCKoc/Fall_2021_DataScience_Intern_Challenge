# Author: Murat C Koc
## Objective: Calculate Shopify Sneaker Stores AOV
## Challenge: Shopify Data Science Internship - Fall 2021

### Question 1:
On Shopify, we have exactly 100 sneaker shops, and each of these shops sells only one model of shoe. We want to do some analysis of the average order value (AOV). When we look at orders data over a 30 day window, we naively calculate an AOV of $3145.13. Given that we know these shops are selling sneakers, a relatively affordable item, something seems wrong with our analysis. 

1. Think about what could be going wrong with our calculation. Think about a better way to evaluate this data. 
2. What metric would you report for this dataset?
3. What is its value?

### Answers:
1. Store_id 78 price per item is 25725 which skew the data. Additionally, automated orders of user_id 607 from store_id 42 with 352 price per item also push the AOV higher values. 
In order to mitigate the effects of extreme outliers, such as store 78 and user_id 607 from the analysis, we need to exclude the store 78 from the data set.

2. Median would be a better metric for that type of skewed data sets.

3. $284.0

### Question 2 answer is at the end of jupyter notebook.