============================================================
  MOVIE RECOMMENDER SYSTEM
  Assignment: Development of a Recommender System
============================================================

STUDENT INSTRUCTIONS:
  Fill in your Registration Number and Name in the ZIP filename:
  RegNo_Name_RecommenderSystem.zip

------------------------------------------------------------
DATASET
------------------------------------------------------------
Dataset : MovieLens 100K
Source  : https://grouplens.org/datasets/movielens/100k/

HOW TO DOWNLOAD:
  1. Go to https://grouplens.org/datasets/movielens/100k/
  2. Click "ml-100k.zip" to download
  3. Unzip it — you will get a folder called "ml-100k"
  4. Place the "ml-100k" folder in the SAME directory as
     the notebook (movie_recommender.ipynb)

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
EXPECTED OUTPUT
------------------------------------------------------------
The notebook will produce:

  Console output:
    - Dataset summary (users, movies, ratings, sparsity)
    - SVD training confirmation
    - Full evaluation table (RMSE, MAE, Precision@10, Recall@10, NDCG@10)
    - Top-10 recommendations for Users 1, 50, and 200
    - Final summary block

  Saved image files:
    - eda_plots.png               → 4-panel EDA visualisation
    - evaluation_results.png      → Bar charts for Top-N metrics
    - rating_prediction_results.png → RMSE/MAE comparison
    - user_recommendations.png    → Recommendations for 3 users

  Typical runtime: 2–4 minutes (SVD training + evaluation loop)

------------------------------------------------------------
ALGORITHMS IMPLEMENTED
------------------------------------------------------------
  1. SVD (Matrix Factorization)   — Collaborative Filtering
  2. Cosine Similarity on Genres  — Content-Based Filtering
  3. Weighted Hybrid (70% SVD + 30% CB) — BONUS

Baselines compared:
  - Most Popular
  - Global Average

------------------------------------------------------------
SUBMISSION ZIP STRUCTURE
------------------------------------------------------------
RegNo_Name_RecommenderSystem.zip
├── movie_recommender.ipynb
├── ml-100k/
│   ├── u.data
│   ├── u.item
│   └── u.user
├── README.txt
└── presentation.mp4

------------------------------------------------------------
VIDEO SCRIPT OUTLINE (3 MINUTES)
------------------------------------------------------------
  0:00–0:30  Problem & domain introduction
  0:30–1:00  Dataset description (show EDA plots)
  1:00–1:45  Algorithm explanation (SVD + Content-Based + Hybrid)
  1:45–2:30  Evaluation results (show comparison table + charts)
  2:30–3:00  Live demo (scroll through recommendations for 3 users)

============================================================
