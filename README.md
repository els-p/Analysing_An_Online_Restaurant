# Analysing An Online Restaurant
Applying data science on a real world business case.

## Background
This project was completed as part a capstone project for the Data Science Immersive course I enrolled myself in. It is a chance to put all I've learnt in 12 weeks into a project of my choice that would reflect my understanding of the topics.

## Data Collection
Source: The data was very kindly given to me by a Singapore online restaurant. 
<br>
The data was given to be in mainly five files:
1. User information
2. Delivery information
3. Order details
4. Menu information
5. Analysis metrics
<br>
As an NDA was signed, parts of the information are censored. Please reach out to me at els.pse+gh@gmail.com if you have any questions or would like to offer feedback and comments!

## Problem Statement
A wealth of transaction data is collected by the Food & Beverage industry. What are some possible outcomes from analysis of the available data?

## Goal
To apply data science concepts to uncover opportunities that can increase revenue. 

## Data Cleaning and Pre-Processing
Actual data from a live business is very dirty. 
<br>
Some of the issues I faced include:
* Columns with multiple data types
* Missing values
* Duplicate columns with similiar but inconsistent information 
* Impossible/extreme values e.g. negative age, invalid postal codes
* Inconsistent definition of labels

## Business Analysis
I first used descriptive statistics to get a sense of the business situation and find a direction to a problem statement I could work on.
<br>
<br>
I found that while the number of orders peaked in 2018, average order amount loss 35% value compared to a year before. Since sales is a function of price and quantity, I look at both factors to find answers. I plotted the average price on the menu and the average price of items purchased by users and found that both had increased marginally. Hence, order value did not decrease because users were purchasing lower-priced items. I found an answer in quantity per order. <em> Users were placing more orders but each order has less items. </em>

## Increasing Revenue by Increasing Order Value
I used PCA and K-Means Unsupervised Clustering to segment customers by purchase behaviour and products by characteristics. <br>
<br>
Alternating Least Squares Method was used to build a recommender system for personalised product recommendations. Upon evaluation of the model, I found that the baseline popularity recommender scored higher. The scores were close (0.88 VS 0.93) so it would be worth validating the personalised recommendations via A/B testing. 
<br>
<br>
I also build a popularity recommender system using Turi Create to find the best-selling items. This would be useful in a cold-start scenario where there is no purchase history for a new user. 

1. Develop customised strategies to target customer segments
2. Identify groups of users who are the <em>low hanging fruits</em> to target for marketing efforts
3. Capture more value from products



