# BANKMARKETING
Based on comprehensive analysis of 41,188 customer contacts with an 11.27% overall conversion rate, the following strategic recommendations are prioritized by impact and implementation difficulty.
# ADULT-ANALYSIS-
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
## Adult lives
### Dataset Preview
#### This dataset contains demographic, educational, occupational, and financial information about adults in the United States. It is often used for income classification analysis, where the main goal is to determine whether an individual earns more than $50,000 per year based on their personal attributes.
## Dataset Description
                                                                             
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
+ What is the total Male Adult?
+ What is the total Female Adult?
+ What is the camparison between Income and Age?
+ What is the average of capital loss by education?
+ What is the average hours per week by income
+ What is the top 10 oldest adult in the dataset?

# Objectives
+ To identify key demographic and socioeconomic factors that influence an individual’s income level (whether they earn more than $50K per year).

+ To analyze the relationship between variables such as education, age, occupation, marital status, and work hours on income distribution.

+ To compare income levels across genders, races, and countries, highlighting patterns of inequality or imbalance.

+ To evaluate the impact of education and work experience on earning potential and economic stability.

+ To explore employment trends — determining which work classes and occupations are associated with higher income levels.

+ To build a predictive model capable of classifying individuals into income categories (≤50K or >50K) based on their demographic and professional features.

+ To provide data-driven insights and recommendations for policymakers, businesses, or individuals aiming to improve income equity and workforce planning.
---
## Tools Used
+ POWER BI
+ SQL
+ PYTHON
---

## Python
+ https://ibb.co/NdCD3N5C
+ from matplotlib.pyplot import xlabel, ylabel


+ try:
    with open('adult.csv', 'r', encoding='utf-8') as f:
        data = f.read()
        print(data)
   + except FileNotFoundError:
    print("Error: adult.csv file not found in the current directory")
+ except PermissionError:
    print("Error: Permission denied when trying to read adult.csv")
+ except UnicodeDecodeError:
    + Try with a different encoding if UTF-8 fails
  +  try:
        with open('adult.csv', 'r', encoding='latin-1') as f:
            data = f.read()
            print(data)
   + except Exception as e:
        print(f"Error reading file with alternative encoding: {e}")
+ except Exception as e:
    print(f"An error occurred: {e}")

   +try:
    import pandas as pd
    import matplotlib.pyplot as plt
    + Read the CSV file
    df = pd.read_csv('adult.csv')
    df['education'] = df['education'].astype('category')
    plt.figure(figsize=(15, 8))
    avg_age = df.groupby('education')['age'].mean()
    bars = plt.bar(avg_age.index, avg_age.values)
    colors = ['red', 'blue', 'green', 'orange', 'purple', 'cyan', 'magenta', 'yellow', 'pink', 'brown', 'gray', 'gold', 'navy', 'teal']
    bars = plt.bar(avg_age.index, avg_age.values, color=colors[:len(avg_age)])
    
     + Add text labels on top of each bar
    for bar in bars:
        height = bar.get_height()
        plt.text(bar.get_x() + bar.get_width()/2., height,
                f'Age: {height:.1f}',
                ha='center', va='bottom')
    
    plt.title('Average Age by Education Level', fontsize=14, pad=20, color ='blue', backgroundcolor='lightgray')
    plt.xlabel('Education Level', fontsize=12)
    plt.ylabel('Average Age', fontsize=12)
    
    +  Rotate x-axis labels for better readability
    plt.xticks(rotation=45, ha='right')
    
    + Adjust layout to prevent label cutoff
    plt.tight_layout()

    plt.show()
except FileNotFoundError:
    print("Error: 'adult.csv' file not found. Make sure it's in the same directory as your Python script.")
except pd.errors.EmptyDataError:
    print("Error: The CSV file is empty.")
except Exception as e:
    print(f"An error occurred: {e}")

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


