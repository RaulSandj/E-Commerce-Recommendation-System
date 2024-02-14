# E-Commerce Recommendation System
Product Recommendation System is a machine learning-based project that provides personalized product recommendations to users based on their browsing and purchase history. The system utilizes collaborative filtering and content-based filtering algorithms to analyze user behavior and generate relevant recommendations. This project aims to improve the overall shopping experience for users, increase sales for e-commerce businesses.<br/>
Dataset from [Kaggle](https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation).

## Cold Start Problem
The cold start problem is a challenge faced by recommender systems. It occurs when a recommender system does not have enough information to make recommendations for a new user or item.
There are two main types of cold start problems:
- User cold start: This occurs when a new user signs up for a service and the recommender system does not have any information about their past behavior.
- Item cold start: This occurs when a new item is added to a service and the recommender system does not have any information about how other users have rated it.

The cold start problem refers to the challenge of making recommendations for new users or items that have little or no interaction data. There are several approaches to addressing this problem:
- Rank-based recommendations: For new users, you can recommend popular items based on their overall popularity or average rating. This approach doesn’t require any information about the user’s preferences and can help introduce them to popular items on the platform.
- Content-based filtering: For new items, you can use content-based filtering to make recommendations based on the item’s attributes or metadata. This approach doesn’t require any interaction data and can help introduce new items to users with similar preferences.
- Hybrid approaches: You can combine multiple approaches to address the cold start problem. For example, you can use rank-based recommendations for new users and content-based filtering for new items.

Here are some specific examples of how the cold start problem can be addressed:
- User cold start: One way to address the user cold start problem is to use collaborative filtering. Collaborative filtering works by finding users who have similar interests to the new user and then recommending items that those users have rated highly.
- Item cold start: One way to address the item cold start problem is to use content-based filtering. Content-based filtering works by analyzing the content of an item and then recommending items that are similar in content.
- Hybrid approaches: Hybrid approaches combine collaborative filtering and content-based filtering to make recommendations. Hybrid approaches can be more effective than either collaborative filtering or content-based filtering alone.

## Modelling
### **1. Rank Based Product Recommendation**
**Objective**
- Recommend products with highest number of ratings.
- Target new customers with most popular products.

**Outputs**
- Recommend top 5 products with 50/100 minimum ratings/interactions.

**Approach**
- Calculate average rating for each product.
- Calculate total number of ratings for each product.
- Create a DataFrame using these values and sort it by average.
- Write a function to get 'n' top products with specified minimum number of interactions.
