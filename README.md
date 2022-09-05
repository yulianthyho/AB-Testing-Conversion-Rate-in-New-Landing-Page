# A/B Testing : Is The New Landing Page Better than The Old One ? 💭👀
Successfully help the company to validated whether the new landing page will give a better conversion rate before rolling out to a bigger audience. With A/B testing, the company can decide to keep using the old one because the result shows that there is no significant differences in conversion rate between the old and the new landing page.

-	Tools: Python (hypothesis testing)
- See my code [here](https://colab.research.google.com/drive/1HN2pTPxcpEjw_vctCqFFQa9Sauj9n5RJ)

## Overview 
An e-commerce company is revamping a new landing page. The company want to experiment whether the new landing page will give better conversion rate before rolling out to a wider audience.

## About the dataset
We were given the experiment result from control and experimental/treatment group. We have hypothesis that the new page (treatment group) will give a better conversion rate.

## Goal
Help company in deciding which landing page is better (keep the old page or implement the new one)

## Exploratory Data Analysis (EDA)
Split the data into 2 groups based on this 2 condition
- Condition 1: control group must receive old landing page only
- Condition 2: treatment group must receive new landing page only

Result :
- The number of user in both group is quite balanced (around 2500 users)
- The conversion rate in treatment group (new landing page) is slightly higher than the conversion rate in control group (old landing page). **But is this difference significant enough?** In order to identify the difference, **A/B hypothesis testing should be done first**

## A/B Testing
We can use Z-test for the hypothesis testing ( number of sample is 2500 , which is > n_sample 30 ).

Our hypothesis are:

Ho : Convension rate in the new landing page is the same to the conversion rate in old landing page.

H1 : Convension rate in the new landing page is difference than the conversion rate in old landing page.

## Insight and Recommendation
(Z-score = 0.584, p-value = 0.558) 

**Result:**

The p_value > 0.05, we do not have enough evidence to reject null hypothesis. It means that the convension rate between new landing page and old landing page is **same** or it doesn't give better conversion rate than the old one (fail to reject the null hypothesis)

**Recommendation**

Since there is no difference between the convension rate in both landing page, the company can keep the old one to save the budget, while do improvement to increase the convention rate.






 
