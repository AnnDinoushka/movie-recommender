MOVIE RECOMMENDER SYSTEM

------------------------------------------------------------
DATASET
------------------------------------------------------------
Dataset : MovieLens 100K
Source  : https://grouplens.org/datasets/movielens/100k/

Key files inside ml-100k/:
  u.data   → 100,000 ratings (user_id, movie_id, rating, timestamp)
  u.item   → 1,682 movies with title + genre flags
  u.user   → 943 users with age, gender, occupation

------------------------------------------------------------
REQUIRED LIBRARIES
------------------------------------------------------------
Install all dependencies with:

  pip install pandas numpy scikit-learn scikit-surprise matplotlib seaborn

Tested on Python 3.9+

------------------------------------------------------------
HOW TO RUN
------------------------------------------------------------
1. Install the required libraries (see above)
2. Download and place the ml-100k/ folder (see DATASET section)
3. Open Jupyter Notebook:
     jupyter notebook movie_recommender.ipynb
4. Run ALL cells from top to bottom:
     Kernel → Restart & Run All


------------------------------------------------------------
ALGORITHMS IMPLEMENTED
------------------------------------------------------------
  1. SVD (Matrix Factorization)   — Collaborative Filtering
  2. Cosine Similarity on Genres  — Content-Based Filtering
  3. Weighted Hybrid (70% SVD + 30% CB) — BONUS

Baselines compared:
  - Most Popular
  - Global Average
