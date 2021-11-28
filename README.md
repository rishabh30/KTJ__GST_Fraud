

#### Project Title

# KTJ GST Fraud Detection (10-15 Jan 2020)

### Overview
Our objective is to build a predictive model that will help us to predict whether a given firm (business entity) is involved in GST fraud. We built this model using features based on different sectors (restaurant, electronics, etc), output tax, month 
and year of bill generated (as it will help to predict which month is more prone to fraud) and the amount of bill generated. We constructed a data set with columns (features) mentioned in Table below. Each row of this data set corresponds to a firm. 


## Project structure
├── data\
├── main.ipynb\
├── submissions\
├── requirements.txt\
└── License

### Prerequisites


```bash
pip install -r requirements.txt
```


### Data Gathering 
We gathered the data from the various news articles from sources like economic times, ministry of corporate affairs, etc. including our dominos bills :)

### Feature Data Extraction Technique and Pre-Processing
- In data pre-processing, we have encoded various sectors into labels and predicted the likelihood of fraud depending on the type of firm.
- Here, from our model what we are trying to do is, gather important features from the bills and we will then predict the likelihood of GST fraud depending on the features from that generated model.
- This model will be able to help the Income Tax officers to focus more on those firms who are more likely to commit a GST fraud as predicted by our model.

### Machine Learning Algorithms
- We used logistic regression to find a relationship between features and the probability of a particular outcome. Logistic regression is an estimation of Logit function. Logit function is simply a log of odds in favor of the event. This function creates an S-shaped curve with the probability estimate, which is very similar to the required stepwise function.
- We have used the correlation matrix to quantify the degree to which two variables are related.
- After analyzing them we removed the unnecessary features to build a better model that would work on a large scale.
- We have used 20% of our model for validation set and obtain an accuracy of around 89.69%. Our final model is an ensemble model of the Gradient Boosting Classifier and Logistic Regression. In the Gradient Boosting Classifier model F1 score is used to find similarity between two clusters.

## Authors 
- [Arpit Raj](https://github.com/)
- [Aayush Biltharia](https://github.com/)
- [Rishabh Singhal](https://github.com/rishabh30) 