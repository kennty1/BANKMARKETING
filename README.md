# BANKMARKETING
Based on comprehensive analysis of 41,188 customer contacts with an 11.27% overall conversion rate, the following strategic recommendations are prioritized by impact and implementation difficulty.
+ [Dataset Preview](#Dataset-Preview)
+ [Dataset Description](#Dataset-Description)
+ [Analytic Questions](#Analytic-Questions)
+ [Objectives](#Objectives)
+ [Tools Used](#Tools-Used)
+ [Python](#Python)
+ [SQL Queries](#sql-queries)
+ [Power Bi Dashboard](#Power-Bi-Dashboard)
+ [Findings](#Findings)
+ [Recommendation](#Recommendation)
---
## Bank Marketing
### Dataset Preview
#### This dataset contains 41,188 records of a bank’s direct marketing campaign, capturing customer demographics, financial status, contact details, previous campaign interactions, and economic indicators, with the goal of predicting whether a client subscribed to a term deposit (y)
## Dataset Description
                                                                             
| **Column**        | **Meaning**                                                                               |
| ----------------- | ----------------------------------------------------------------------------------------- |
| age               | Age of the client                                                                         |
| job               | Type of job (admin, technician, services, etc.)                                           |
| marital           | Marital status (married, single, divorced)                                                |
| education         | Education level                                                                           |
| default           | Has credit in default? (yes/no)                                                           |
| housing           | Has housing loan? (yes/no)                                                                |
| loan              | Has personal loan? (yes/no)                                                               |
| contact           | Contact communication type (cellular/telephone)                                           |
| month             | Last contact month of year                                                                |
| day_of_week       | Last contact day of the week                                                              |
| duration          | Last contact duration (in seconds)                                                        |
| campaign          | Number of contacts performed during this campaign                                         |
| pdays             | Number of days since last contact from previous campaign (999 = not previously contacted) |
| previous          | Number of contacts performed before this campaign                                         |
| poutcome          | Outcome of previous marketing campaign                                                    |
| emp.var.rate      | Employment variation rate (quarterly indicator)                                           |
| cons.price.idx    | Consumer price index (monthly indicator)                                                  |
| cons.conf.idx     | Consumer confidence index (monthly indicator)                                             |
| euribor3m         | Euribor 3-month rate (daily indicator)                                                    |
| nr.employed       | Number of employees (quarterly indicator)                                                 |
| y                 | Has the client subscribed to a term deposit? (yes/no)                                     |


---
# Analytic Questions
+ What is the overall campaign success rate and how many customers suscribed?
+ How does campaign success vary by month and days of the week?
+ Which customer demographics have the highest conversion rates?
+ What is the distribution of customers who subscribed vs those who didn't(success/failure)?

# Objectives
+ Measure Overall Campaign Performance:
Determine the total number of customers who subscribed.
Calculate the overall campaign success rate (conversion rate).
+ Evaluate Campaign Performance by Time:
Analyze how subscription rates vary across different months.
Examine differences in campaign success by day of the week.
+ Identify peak periods with the highest conversion rates:
Identify High-Performing Customer Segments
Assess which demographic groups (age, job, marital status, education, etc.) have the highest subscription rates.
Discover customer profiles most likely to convert.
+ Analyze Subscription Distribution:
Compare the proportion of customers who subscribed versus those who did not.
Understand the imbalance between success and failure outcomes.

---
## Tools Used
+ POWER BI
+ SQL
---



##  SQL Queries
### https://ibb.co/yBQzRDkQ
### https://ibb.co/4nFJ7Ck3
### https://ibb.co/j9Bcvsz2
### https://ibb.co/tPnDQmX8
### https://ibb.co/v6sggByr
### https://ibb.co/chMNvRW5
### https://ibb.co/rRyKyngs


##  Power Bi 
### https://ibb.co/k6g2zN35
### https://ibb.co/fVQqGxVq
### https://ibb.co/wZD48rn0
### https://ibb.co/ZRxSMrxF

---

# Findings
+ ## Overall Campaign Performance
### Total customers: 41,188
### Customers subscribed: 4,640
### Overall success rate: ≈11.3%
### The campaign conversion rate is relatively low, meaning nearly 9 out of 10 customers did not subscribe.

+ ## Campaign Success by Month & Day
  ## By Month:
### Certain months (especially March, September, October, and December) typically show higher conversion rates.
### Months with heavy outreach (like May) may have many contacts but lower conversion efficiency.
### This suggests timing plays a strong role in campaign success.

## By Day of Week:
### Conversion differences across weekdays are usually moderate.
### Mid-week days (Tuesday–Thursday) often perform slightly better than Mondays and Fridays.
### Day of contact has some influence, but not as strong as month or customer profile.

+ ## Customer Demographics with Higher Conversion
## Age:
### Middle-aged and older clients tend to subscribe more than very young customers.
## Job Type:
### Retired clients and students often show higher subscription rates.
### Blue-collar and services roles may have lower conversion rates.
## Marital Status:
### Married individuals often make up the largest subscriber group.
## Education:
### Customers with higher education levels sometimes show better engagement.

+ ## Distribution of Success vs Failure
### No (Failure): ~88.7%
### Yes (Success): ~11.3%

# Recommendation
## 1. Improve Targeting Strategy
+ Focus on high-performing demographic segments (retired, middle-aged, previously successful contacts).
+ Use predictive modeling to identify high-probability customers.

## 2. Optimize Campaign Timing

+ Increase marketing efforts during high-performing months.
+ Schedule more calls mid-week for better engagement.
+Reduce heavy campaigns in low-performing periods.

## 3. Reduce Campaign Fatigue
+Avoid excessive repeated contacts.
+Limit number of calls per customer.
+Prioritize quality conversations over quantity.

## 4. Leverage Previous Campaign Success
+Customers with previous successful outcomes should be prioritized.
+Build loyalty campaigns for previously converted customers.

# Conclusion
+ The campaign currently has a low overall conversion rate (11.3%), but there are identifiable high-performing customer segments and time periods.


