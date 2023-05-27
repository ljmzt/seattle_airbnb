# Airbnb vs Rent -- which is better in Seattle

## Project Motivation
This is part of the Udacity nanodegree requirements. My goal is to examine whether or not Airbnb is more profitable compared to long term rental. This is the github repo accompanying my medium post. In particular, I would like to know:
* Q1: Is Airbnb more profitable than rent in general?
* Q2: How to become a good host of Airbnb?
* Q3: Is there a particular season during the year that one should concentrate on?

## Main Files
1. seattle-airbnb-lumped-together:  
This is the notebook for grading. It is assembled from the original notebooks.

2. check-rent.ipynb:  
This is the file that converts the fair market rents (FMR) from the U.S. Department of Housing and Urban Development (HUD) to an estimate of rent for a given zipcode and number of bedrooms. Please refer to the notebook for sources of data.

3. Q1--revenue-vs-rent:  
This is the file that computes the revenue and compare that with rent. Please see the notebook for exactly how to inflate the proxy revenue. 

4. Q2--what makes it a good listing--EDA.ipynb and Q2--modeling.ipynb:  
These two answer the question: for given zipcode and bedrooms numbers, what can be done to improve the profit. The EDA notebook has length discussion on each feature, pay attention to the has\_pet feature, which is inferred from the reviews file. When doing the linear modeling, it's important to drop one column when making dummies to avoid linear dependence. While most people will choose to drop first, I choose to drop the one with most counts. This is for better inrepretation, i.e. what needs to be changed compared to what most of the other people are doing in order to make more profit.  

## Libraries used
* python==3.9.13
* pandas==1.4.0
* numpy==1.23.3
* matplotlib==3.5.1
* seaborn==0.11.2
* scipy==1.9.1
* scikit-learn==1.0.2

## Acknowledgement

