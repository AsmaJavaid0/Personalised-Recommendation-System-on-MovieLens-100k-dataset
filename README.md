# Personalised-Recommendation-System-on-MovieLens-100k-dataset

This project is a beginner-to-intermediate level movie recommendation system built as part of an AI Internship task. It uses **collaborative filtering** to recommend movies to users based on their preferences and similarities with other users.

---

## 📌 Objective

Build a basic movie recommendation system using **collaborative filtering** (user-based), applying **cosine similarity** to suggest movies that a user is likely to enjoy.

---

## 📂 Dataset

- **Source:** [MovieLens 100k dataset](https://grouplens.org/datasets/movielens/100k/)
- **Used Files:**
  - `u.data` – contains user ratings for movies
  - `u.item` – contains movie titles and metadata

---

## 🛠️ Technologies Used

- **Python**
- **pandas** – data manipulation
- **numpy** – numerical computations
- **sklearn** – for cosine similarity
- **kagglehub** – to download dataset from Kaggle

---

## 🧠 Approach

1. **Data Loading:**
   - Loaded the MovieLens dataset using `kagglehub`.
   - Merged user ratings with movie titles.

2. **Data Preparation:**
   - Created a user-item rating matrix using `pivot_table`.
   - Filled missing ratings with `0` to simplify similarity computation.

3. **Similarity Calculation:**
   - Used `cosine_similarity` to find similarities between users.

4. **Recommendation Logic:**
   - Identified the most similar user.
   - Recommended top-rated movies from that user which the current user hasn't watched.

5. **Output:**
   - Displayed at least 3 personalized recommendations for a sample user.

---

## 🎯 Sample Output

```text
Recommendations for User 1:
- Contact (1997)
- The Saint (1997)
- Air Force One (1997)
