# cookies-linreg
Predicting Chocolate Chip Cookie Recipe Ratings Using Linear Regression

The purpose of this project was to use linear regression in order to predict chocolate chip cookie recipe ratings on allrecipes.com. The main focuses of this project were to improve web scraping skills and to use linear regression models effectively. The initial hope was to be able to determine whether specific ingredients or relationships between ingredients have predictive power when it comes to chocolate chip cookie recipe ratings, since reviews often comment about ratios between ingredients such as butter and flour. However, initial exploratory data analysis quickly reveals that ratings on allrecipes.com are highly left skewed and that correlations between individual features vs the target were very low. Polynomial features was also used in an attempt to discover any higher order relationships. OLS, LASSO, Ridge, regressions were attempted, with the best model resulting in a holdout-set R^2 of 0.06. Random Forest Regressor yielded a slightly better result, with a holdout-set R^2 of 0.146. 

Takeaways from this project are:
1. 1-5 scale is not continuous and therefore not great for linear regression
2. Ratings should not be calculated merely using a simple average, as recipes with 20k ratings and recipes with 5 ratings can yield the same rating
3. Ratings are very subjective in nature

Future work includes:
1. Conducting sentiment analysis of reviews as features
2. Modifying the ratings by taking the number of ratings into account
3. Use classification instead of linear regression in order to classify good/bad recipe instead of predicting rating
