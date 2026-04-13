# Amazon Product Recommendation System

## Project Overview
This project builds a recommendation system for Amazon products using collaborative filtering and deep learning techniques. The goal is to predict user preferences and recommend relevant products.

## Dataset
The dataset contains user-item interactions including:

- User ID
- Product ID
- Rating
- Timestamp

This structure is suitable for collaborative filtering models.

## Exploratory Data Analysis

Key findings:

- The dataset is highly sparse
- Most users rate only a few products
- Rating distribution is skewed toward high ratings
- User activity increases over time

These findings guide model selection.

## Models Implemented

We implemented multiple recommendation approaches:

- Baseline Model (Popularity-based)
- Recent Model (Trending items)
- SVD (Matrix Factorization)
- Neural Collaborative Filtering (Deep Learning)
- Hybrid Model (SVD + Baseline)

## Model Performance

| Model | RMSE | MAE |
|------|------|------|
| SVD | 1.2688 | 0.9932 |
| Hybrid | 1.2707 | 1.0041 |
| Baseline | 1.2743 | 1.0059 |
| Recent | 1.3353 | 1.0434 |
| NeuralCF | 1.7908 | 1.2923 |

## Final Model

SVD achieved the best performance and was selected as the final recommendation model.

## Example Recommendation

Top 5 recommended items for a user:

- Item A
- Item B
- Item C
- Item D
- Item E

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Surprise
- TensorFlow

## Future Improvements

- Deploy recommendation system
- Use larger dataset
- Add hybrid ranking models
