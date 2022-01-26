# Coffee-business-Analysis

In this project, we extracted coffee business details and reviews from Yelp dataset. We analyzed attributes and services that a coffee shop might offer which can improve the ratings of their businesses.s

# Summary 
* coffee_business_rev_extraction - extracting business IDs and reviews from Yelp Dataset pertaining to coffee shops;
* coffee_business_analysis - analysis of coffee business ratings;
* Glove_model - Used pretrained Glove embeddings on coffee reviews and classified them into positive and negative/neutral reviews.

## Locations of coffee shops across North America

In the dataset, the coffee shops were located in North America mostly in the United States.

<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/map.png" width="500" height="300">

## Distribution of our Dataset

Most of the coffee shops have ratings between 3.5 and 4.5.

<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/count_of_rests.png" width="500" height="300">


## Attributes vs Ratings

We extracted some of the attributes and services a restaurant might offer and compared them to their average ratings. We noticed lower price-range and quieter coffee shops tend to have higher ratings.


<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/Ratings_vs_attr.png" width="900" height="300">


Coffee shops with higher reviews counts and those open for shorter daily hours tend to have higher ratings.

<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/review_counts_vs_ratings.png" width="500" height="400">  </img>
<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/daily_hours_ratings.png" width="500" height="400">


## Predicting ratings using attributes and features

For coffee shops with ratings less than 4, we ranked them as a "Low/Average" rated and those with ratings 4 and above we ranked them "High" rated.

We used a Random forest classifier model to predict these rankings. Below is the picture of feature importance using this model. We observe "review_counts" and "daily_hours" have significantly higher feature importances.

<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/feature_importance.png" width="900" height="600"> 

We obtained an accuracy of 76% and f1_macro average of 76%. Here is the normalized confusion matrix.

<img src="https://github.com/mitabanik/Coffee-business-reviews/blob/main/img/confusion_matrix.png" width="400" height="300"> 









