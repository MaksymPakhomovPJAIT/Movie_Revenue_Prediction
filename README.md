# Movie_Revenue_Prediction 

---

This project focuses on **predicting the worldwide gross revenue** of movies based on various features such as **budget, ratings, nominations, awards, director success, and actor popularity**. Using **machine learning models** like **Random Forest and XGBoost**, the goal is to estimate a film's box office earnings and analyze which factors contribute the most to its success.  

## Features & Approach  

- **Dataset**: IMDb movie data (1960–2024), including **budget, genres, director, actors, country, duration, awards, and ratings**.  
- **Target Variable**: `Worldwide Gross`.  
- **Handling Missing Data**:  
  - **Budget**: Imputed using Regression-based imputation.  
  - **Other Features**: Imputed using yearly and genre-based averages.  
- **Feature Engineering**:  
  - Actor popularity, director ranking, country index, and more.  
  - Label encoding for categorical variables (e.g. MPA).  
- **Models Used**:  
  - **Random Forest** – for robust performance and feature importance analysis.  
  - **XGBoost** – for fine-tuned predictions.  
- **Evaluation Metrics**:  
  - R² score.  
  - Mean Squared Error (MSE).  


## Results & Insights  

- Actors, directors and budget had a **significant** impact on revenue predictions.  
- Budget could be used as a key predictor **only when the main country was the United States** (due to currency inconsistencies).
- Revenue can be predicted by selected feature with a relatively high accuracy.  

## Future Improvements  

- Using **deep learning** models (e.g., LSTMs for sequential analysis of box office trends).  
- Improve budget imputation using **historical inflation adjustments**.  
- Explore **ensemble stacking** for better predictive performance.  
