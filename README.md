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
+ Education plays a major role in income level — individuals with higher education (especially Bachelor’s degree and above) are more likely to earn above $50K annually.

+ Age and work experience positively correlate with income — older individuals, particularly those between 35–55 years, tend to have higher earnings.

+ Gender income disparity exists — males are more likely to earn > $50K compared to females, even when holding similar education or job levels.

+ Marital status influences income — married individuals, especially those in “Married-civ-spouse” status, have a higher probability of earning > $50K than single or divorced individuals.

+ Occupation type matters — high-income individuals are more concentrated in occupations like Exec-managerial, Prof-specialty, and Tech-support, while lower-income groups are common in Service and Labor roles.

+ Work hours per week impact earnings — people who work more than 40 hours per week tend to fall into the higher income category.

+ Capital gain/loss is a strong indicator of wealth — those with significant capital gains are much more likely to earn > $50K.

+ Racial imbalance is visible — the majority of higher-income earners are from the White racial group, indicating potential socioeconomic disparities.

+ Country of origin has minimal effect — most individuals in the dataset are from the United States, with minimal variation in income trends by country.

+ The dataset is slightly imbalanced — a larger percentage of individuals earn ≤ $50K, showing that high-income earners form a minority group.

# Recommendation
+ Promote higher education and skill development

+ Since education strongly influences income, government and organizations should invest in accessible education, professional certifications, and technical training to help individuals move into higher-paying roles.

+ Encourage equal employment opportunities

+ The gender gap in income suggests the need for fair hiring practices, salary transparency, and gender equality programs in workplaces.

+ Support continuous career growth

+ Employers should provide career development plans, mentoring, and upskilling programs to help workers advance into managerial or technical positions that pay higher salaries.

+ Address work-life balance while maintaining productivity

+ Although longer working hours are linked to higher income, companies should ensure balanced workloads and introduce flexible work options to maintain employee well-being.

+ Empower marital and family support programs

+ Since marital stability shows a link with higher income, governments and communities can offer family financial planning and support programs to promote economic stability.

+ Focus on economic inclusion and diversity


