# Ex-09-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
STEP 1:Read the given Data

STEP 2:Clean the Data Set using Data Cleaning Process

STEP 3:Apply Feature generation and selection techniques to all the features of the data set

STEP 4:Apply data visualization techniques to identify the patterns of the data.

# CODE
```
Name: PRADEEPASRI S
Reg.No: 212221220038
```
```
import seaborn as sns
import matplotlib.pyplot as plt
tips=sns.load_dataset('tips')
tips

tips.head()

tips.info()

sns.barplot(x='day',y='total_bill',data=tips)
plt.title("Weekly highest total bill amount")

sns.barplot(x='smoker',y='tip',data=tips, palette='rainbow')
plt.title("Average tip amount given by smokers and non-smokers")

sns.boxplot(x='size', y='tip',data=tips)
plt.title("Tip percentage based on the sizes of the dining party")

sns.boxplot(x='sex', y='tip',data=tips)
plt.title("Higher tips based on gender")

plt.plot(tips['day'],tips['total_bill'])
plt.title("Relationship between the total bill amount and the day of the week")
plt.show()

sns.violinplot(x='time',y='total_bill',data=tips)
plt.title("Distribution of total bill amounts vary across different time periods(lunch vs. dinner)")

sns.barplot(x='size',y='total_bill',data=tips)
plt.title("Highest average total bill amount based party size")

sns.boxplot(x='day',y='total_bill',data=tips)
plt.title("Distribution of tip amounts for each day of the week")

sns.violinplot(x='time',y='tip',data=tips)
plt.title("Tip based on the type of service ")
sns.scatterplot(data=tips, x='total_bill', y='tip')
correlation_coefficient = tips['total_bill'].corr(tips['tip'])
print("Correlation Coefficient:", correlation_coefficient)

tips.corr()
plt.subplots(figsize=(7,5))
sns.heatmap(tips.corr(),annot=True)
```
# OUPUT
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/4e6b5faf-9f10-4e1e-a579-3baa2a2242cd)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/a90beb34-9a73-4570-bc0f-f77b69a3d97d)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/fe417975-ecb6-433a-9a31-331fd11ad8e2)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/fb3f8b7b-b835-4909-859d-89cf1b343494)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/e42c3ecb-093e-44c0-ae19-29db6536127b)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/dd12cde4-db0a-4d5d-8ec3-16e990689dfc)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/f33af1ed-89d1-4b19-9362-d2d879f17a42)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/12d1989b-5346-4375-8647-c494055b450d)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/a9e9caa1-7c20-4c45-83bb-a5c5a59bfd93)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/6464a770-ac76-4756-bcf7-560ac0e67c17)
![image](https://github.com/pradeepasri26/ODD2023-Datascience-Ex-09/assets/131433142/69f80d6a-fd10-4fdc-814b-5dc60de9f1d0)

## RESULT
Hence, Data Visualization is applied on the complex dataset using libraries like Seaborn and Matplotlib successfully based on tips dataset and the data is saved to file.








