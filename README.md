# Book Recommendation System
I love goodreads. As one of the biggest online community for books, it has an active community of members that writes ardent reviews. I also use it to find books to read and record the books I read. For this project, I wanted to create a book recommendation system of my own. I used a 10k-goodreads-dataset and cosine similarity and matrix factorization to create the recommendation system.
___

- model: User-based collaborative filtering + matrix factorization using neural networks
- dataset: [goodreads rating 10k](https://github.com/zygmuntz/goodbooks-10k)
- modules: sklearn, keras

**Outline**:

1. input function for getting rating from a new user
2. calculate the similarity between users and new user using cosine similarity (find the closest user)
3. use matrix factorization to calculate book rating for all the user
4. recommend top 10 books for new user based on similar user's book recommendation from matrix factorization

** You can download the trained embeddings:
- https://flask-uploads.s3.ap-northeast-2.amazonaws.com/pickles/book_norm.npy
- https://flask-uploads.s3.ap-northeast-2.amazonaws.com/pickles/book_rating_emb.h5
- https://flask-uploads.s3.ap-northeast-2.amazonaws.com/pickles/r_norm.npy
- https://flask-uploads.s3.ap-northeast-2.amazonaws.com/pickles/user_norm.npy
___
Check out [my website]() for the full application.

Input: 
![Image description](https://i.imgur.com/unRlcvC.png)

Output:
![Image description](https://i.imgur.com/h9qOCse.png)

**reference**:
* matrix-factorization tutuorials: 
    - https://course.fast.ai/videos/?lesson=4
    - https://medium.com/@jdwittenauer/deep-learning-with-keras-recommender-systems-e7b99cb29929
    - https://towardsdatascience.com/building-a-book-recommendation-system-using-keras-1fba34180699
* user-based collaborative filtering: 
    - https://medium.com/@wwwbbb8510/comparison-of-user-based-and-item-based-collaborative-filtering-f58a1c8a3f1d
    - https://medium.com/sfu-cspmp/recommendation-systems-user-based-collaborative-filtering-using-n-nearest-neighbors-bf7361dc24e0
