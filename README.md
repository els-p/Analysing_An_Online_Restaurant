# Analysing An Online Restaurant
Applying data science on a real world business case.

## Background
This project was completed as part a capstone project for the Data Science Immersive course I enrolled myself in. It is a chance to put all I've learnt in 12 weeks into a project of my choice that would reflect my understanding of the topics.

## Data Collection
Source: The data was very kindly given to me by a Singapore online restaurant. 
<br>
The data was given to me in mainly five files:
1. User information
2. Delivery information
3. Order details
4. Menu information
5. Analysis metrics
<br>
As a non-disclosure agreement was signed, parts of the information are censored. Please reach out to me at <els.pse@gmail.com> if you have any questions or would like to offer feedback and comments!

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

## Models
I used <strong>PCA and K-Means Unsupervised Clustering</strong> to segment customers by purchase behaviour and products by characteristics. 
<br>
<br> 
I grouped users into four buckets using <strong>Recency, Frequency and Monetary Value</strong> metrics to help narrow down users that could be targeted first for a higher return on investment on marketing dollars in the immediate term.
<br>
<br> 
<strong>Alternating Least Squares Method</strong> was used to build a recommender system for personalised product recommendations. Upon evaluation of the model, I found that the baseline popularity recommender scored higher. The scores were close (0.88 vs 0.93) so it would be worth validating the personalised recommendations via A/B testing. 
<br>
<br>
I also build a popularity recommender system using <strong>Turi Create</strong> to find the best-selling items. This would be useful in a cold-start scenario where there is no purchase history for a new user. 

## Business Impact: Increasing Revenue by Increasing Order Value
Using data science, I was able to derive the following outcomes:

1. Develop customised strategies for each customer segment
2. Identify groups of users who are the <em>low hanging fruits</em> to target for marketing efforts
3. Suggest a tweak to loyalty programme to incentivise users to come back sooner
4. Make recommendations to capture more value from products

## Future Development
The project was totally exploratory with minimal discussion with business owners of the online restaurant. Possible future development include:
* Segmenting users into a set number of clusters according to prior knowledge, to achieve business goals 
* Having users rate products so that the ratings can be used to build a recommender system based on item similairity using item-item collaborative filtering
* Collecting more user features e.g. identifying home and office address (for demographic information), birthday (for age) etc.
* Sentiment analysis of reviews


