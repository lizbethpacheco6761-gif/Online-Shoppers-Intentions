# Online-Shoppers-Intentions
For my final project, I decided to use the **Online Shoppers Purchasing Intention Dataset** from UCI's Machine Learning Repository.  
As an avid online shopper, it is interesting to me to see what influences a transaction to go through.


Here is the link to the UCI's website where the dataset is from: https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset


## **Introduction**

For my final project, I decided to use the Online Shoppers Purchasing Intention Dataset from UCI's Machine Learning Repository. The dataset shows customer behaivor during online shopping sessions including visit timing, whether the visitor is new or returning, and how long each session lasts. Each session is labeled as true or false depending if there was a purchase made.

In this project, I will focus on the following questions:

- Which session features influence whether a purchase is made?
- What user behaviors are most associated with completed transactions?
- Can a machine learning model accurately predict whether an online session will result in a purchase?

## **Exploratory Data Analysis**

After importing and reviewing the dataset, the next step is to complete an EDA. The Online Shoppers Purchasing Intention dataset contains over 12,000 online shopping sessions with a mix of numerical and categorical features. The dataset includes information such as page visits, time spent on pages, visitor type, bounce rates, and page values. The target variable, Revenue, indicates whether a session resulted in a purchase. There are no missing values in the dataset.

<img width="692" height="523" alt="image" src="https://github.com/user-attachments/assets/dad557fc-43a2-4a28-a726-eb2214f97720" />

There is a class imbalance in the dataset, most sessions do not result in a purchase.

