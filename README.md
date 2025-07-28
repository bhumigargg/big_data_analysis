# 📊 Big Data Analytics with Apache Spark  
## MovieLens 25M Dataset Analysis

This project performs big data analysis using **Apache Spark** on the **MovieLens 25M dataset**, a large-scale collection of movie ratings by users. It demonstrates Spark's capabilities to handle and analyze large datasets efficiently using SQL-like queries and PySpark DataFrames.

---

## 🛠️ Technologies Used
- **Google Colab** (for cloud-based execution)
- **Apache Spark 3.1.2**
- **PySpark (Spark with Python)**
- **MovieLens 25M Dataset** (from GroupLens)
- **Pandas** (for visualization)

---

## 📂 Dataset Details

- **Source:** [GroupLens MovieLens 25M](https://grouplens.org/datasets/movielens/25m/)
- **Files Used:**
  - `ratings.csv`: userId, movieId, rating, timestamp
  - `movies.csv`: movieId, title, genres
- **Size:** ~25 million ratings from 162,000 users on 62,000 movies

---


## **Download and Load the Dataset:**
    ```python
    !wget https://files.grouplens.org/datasets/movielens/ml-25m.zip
    !unzip -q ml-25m.zip

    ratings = spark.read.csv("ml-25m/ratings.csv", header=True, inferSchema=True)
    movies = spark.read.csv("ml-25m/movies.csv", header=True, inferSchema=True)
    ```

---

