# movie-recommendation-spark
Movie Recommendation System using Spark (ALS)

1. **Project Overview**:
   Objective: Build a personalized movie recommendation system that ensures scalability while handling large-scale, highly sparse data.
   The Problem: Addressed a significant sparsity challenge where only 20M actual ratings existed out of approximately 3.7 billion possible interactions.
  
2. **Data Characteristics**
   Dataset: Utilized the MovieLens 20M dataset.
   Scale: Contained 20,000,263 ratings from 138,493 users across 27,278 movies.
   Rating Scale: 0.5 to 5.0 stars.
   
3. **Technology & Architecture**
   Environment: Implemented an end-to-end pipeline in Databricks.
   Engine: Leveraged Apache Spark and Spark MLlib for distributed processing.
   Workflow: Included data cleaning, an 80-20 train-test split, and Top-N recommendation generation.

4. **Modeling & Results**
   Algorithm: Used Alternating Least Squares (ALS) for collaborative filtering through matrix factorization.
   Latent Features: The model successfully learned latent user and movie features to make predictions.
   Evaluation: Achieved a Root Mean Squared Error (RMSE) of 0.8159.
   Interpretation: On average, predictions deviate by only ~0.82 stars, representing strong performance for a large-scale system
