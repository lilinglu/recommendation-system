# recommendation-system
## Object

Built simple algorithms which aim to provide the most relevant and accurate prodcts to the user by filtering useful stuff from of a huge pool of information base. Recommendation system discovers data patterns in the data set by learning consumers choices and produces the outcomes that co-relates to their needs and interests.

## Problem

### 1 Cold-start problem
* The term “cold start” derives from cars. When the engine is cold, the car is not yet working so smoothly, but once the optimal temperature is reached, it works just fine. For a recommendation engine it simply means that the conditions are not yet optimal for it to operate smoothly and provide best results. There are two major cold start categories: product cold start and customer cold start.

* ways to help recommender systems cope with these issues.

  * Content-based filtering
  * popularity-based filtering.
  * Here I also tried collaborative filtering model.
  
### 2 How to evaluate the models?

* In Recommender Systems, there are a set metrics commonly used for evaluation. We chose to work with Top-N accuracy metrics, which evaluates the accuracy of the top recommendations provided to a user, comparing to the items the user has actually interacted in test set. This evaluation method works as follows:

* For each user
  * For each item the user has interacted in test set
    * Ask the recommender model to produce a ranked list of recommended items, Compute the Top-N accuracy metrics for this user and interacted item from the recommendations ranked list

    * Aggregate the global Top-N accuracy metrics. The Top-N accuracy metric choosen was Recall@N which evaluates whether the interacted item is among the top N items (hit) in the ranked list of recommendations for a user.
