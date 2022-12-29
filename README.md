# Recommendation Systems

‘Customers who bought this, also bought…’ We often come across personalised recommendations while shopping on Amazon, listening to music on Spotify, and binging shows on Netflix, to quote a few. These are so widespread that many of us interact with them without even realising it. All these websites are trying to gauge our tastes to be able to drive continuous engagement. These companies leverage our shopping/listening/watching patterns to predict what we might like in the future. In a way, recommender systems are a win-win for both users and businesses. For users, they offer better experience and engagement, while for businesses, they help increase revenues.

## Collaborative Filtering
There are several approaches to building a recommendation engine. However, we will focus on the collaborative filtering approach. The starting point for collaborative filtering is to have the past interactions between users and items stored in a sparse called the “user-item interaction matrix”. The assumption is that these past user-item interactions are sufficient to detect similar users and/or similar items, and make recommendations based on these computed proximities.

![ratings_matrix (1)](https://user-images.githubusercontent.com/57900104/209997013-2e764e73-7b97-4c7d-ac3d-b5e2e0858bcd.jpg)


Unlike some other techniques, the major advantage of collaborative filtering is that we do not need to know the content in detail. For instance, if you watch Harry Potter movies on Prime Video, it recommends you other movies that were viewed by people who also watched Harry Potter. In this approach, the recommender system may not even care about the genre, cast or director of the movie being suggested. It will simply recommend it because other people with similar tastes watched it.

Collaborative filtering can be categorized into:

**User- based:** Depending on the ratings the users have given to the same items, we try to figure out the users having similar tastes/preferences as user A using cosine similarity. Further, we use weighted sum of ratings provided by the nearest neighbours (that is, like-minded users as A) for an item X and compute the tentative rating that user A may provide to this item.

**Item- based:** In contrast to measuring similarity between users, the item-based approach aims at finding similar items/products. The rating of a user on item X is then predicted by taking the weighted sum of ratings provided by the user on nearest neighbours (in this case - other items similar to item X). Item-based approach is a successful technique that various companies widely use.


Medium Link: https://medium.com/@urvimidha/recommendation-system-using-collaborative-filtering-in-python-83992251c8f7
