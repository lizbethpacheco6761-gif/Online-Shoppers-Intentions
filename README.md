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

<img width="687" height="507" alt="image" src="https://github.com/user-attachments/assets/d0355b3d-d25d-4c57-ac50-3fa49af60d0e" />

The plot above shows that returing customers are more likely to make a purchase when visiting the site.


## **Preprocessing**

Before building the machine learning model, preprocessing steps were applied to prepare the data for the analysis. The following steps ensures features were properly formatted and scaled for the modeling.

- Selected categorical & numerical variables.
- Encoded categorical variables.
- Defined target variable & features.
- Create an 80/20 train-test split.
- Scaled numerical features.

The training data consists of 9,864 sessions with 26 features.

## **Model Implementation**

For the model implementation, **logistic regression** was selected because the problem is a binary classification task. The model provides a strong baseline for predicting whether visitors would complete an online shopping transaction.
<img width="523" height="297" alt="image" src="https://github.com/user-attachments/assets/f277ca82-7bd1-4df1-8936-3a91d69e8b6e" />

## **Model Evaluation**

Since logistic regression was used for this classification task, the model was evaluated using a confusion matrix along with accuracy and F1 score to better assess its performance.

**Confusion Matrix**
<img width="637" height="508" alt="image" src="https://github.com/user-attachments/assets/a3d4ddbe-00a1-43f1-80da-9d3acd4e7173" />

Based on the confusion matrix, the logistic regression model performed well at identifying sessions that did not result in a purchase, which can be due to the class imbalance. The model did struggle to correctly identify all of the sessions that did end in a purchase as reflected by the high number of false negatives.


**Classification Report**
<img width="497" height="173" alt="image" src="https://github.com/user-attachments/assets/a1dc1387-cb9b-4a09-9081-742d9af4e2b1" />

The model achieved an accuracy of **88%** but showed lower recall for purchasing sessions, indicating difficulty identifying all purchases due to class imbalance.


## **Conclusion**
This final project used logistic regression to predict whether an online shopping session would end with a purchase using the **Online Shoppers Purchasing Intention** dataset from UCI's Machine Learning Repository.  Exploratory analysis showed that features like visitor type did influence purchasing behavior, with returning customers being more likely to make a purchase.  
The logistic model achieved an accuracy score of **88%**, indicating that it was effective at identifying patterns in online shopping behaviors.  But there was a lower recall score for the purchasing sessions due to the class imbalance within the dataset.  
Overall, this project demonstrates how machine learning can be used to better understand online customer behavior while also highlighting opportunities for improving model performance.

