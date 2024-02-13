# E-Commerce Recommendation System
Product Recommendation System is a machine learning-based project that provides personalized product recommendations to users based on their browsing and purchase history. The system utilizes collaborative filtering and content-based filtering algorithms to analyze user behavior and generate relevant recommendations. This project aims to improve the overall shopping experience for users, increase sales for e-commerce businesses.
Dataset from [Kaggle](https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation)

## Modelling
### **1. Rank Based Product Recommendation**
**Objective**
* Recommend products with highest number of ratings.
* Target new customers with most popular products.

**Outputs**
* Recommend top 5 products with 50/100 minimum ratings/interactions.

**Approach**
* Calculate average rating for each product.
* Calculate total number of ratings for each product.
* Create a DataFrame using these values and sort it by average.
* Write a function to get 'n' top products with specified minimum number of interactions.
