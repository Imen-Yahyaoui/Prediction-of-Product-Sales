##**Prediction of Product Sales**##

**Author:** Imen YAHYAOUI

**Business problem:**
Make predictions about future sales.

**Data:**
The dataset contains information about products, including their IDs, weights, fat content, visibility in stores, category, and retail prices. It also includes store details like IDs, establishment years, sizes, location types, and types (grocery or supermarket). The target variable is the sales of each product in a specific store. This dataset is valuable for retail analysis and predictive modeling tasks.
The Data used: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

**Methods**

Handling Missing Values:
Missing data can disrupt model training. Impute missing values using median for numerical features,most frequent category for ordinal features, and fill value Missing for categorical features.

Encoding Categorical Variables:
Convert categorical variables into numerical format for machine learning algorithms. Use one-hot encoding for nominal variables and label encoding for ordinal variables.

Feature Scaling:
Normalize feature scales to prevent bias in models sensitive to scale differences. Apply standardization (mean = 0, standard deviation = 1)based on data distribution and algorithm requirements.

**Results**

![Visualisation](https://github.com/Imen-Yahyaoui/Prediction-of-Product-Sales/assets/161170929/249fbfd1-187d-419c-b51f-18e58a3d900e)


The figure displays a visualization of how different types of stores (Outlet_Type) are linked to product sales in these stores (Item_Outlet_Sales), which can help identify trends or significant patterns in the data.

I used the Random Forest model to iteratively train and evaluate different values of n_estimators, storing the R2 scores for training and testing datasets in a DataFrame named scores for analysis and comparison.

Comparing the tuned model to the default Random Forest model:
- The tuned model shows a slightly higher R^2 on the training data (0.94 vs. 0.938), indicating a better fit to the training set.
- However, the R^2 on the testing data for the tuned model (0.56) is slightly lower than that of the default model (0.559), suggesting that the performance did not significantly improve on unseen data.
- The tuned model has a slightly lower MAE on the training data but a slightly higher MAE on the testing data compared to the default model.
- The tuned model has a lower MSE on the training data but a higher MSE on the testing data compared to the default model.
- The tuned model has a lower RMSE on both the training and testing data compared to the default model.

In summary, while the tuned model shows improvements in some metrics on the training data, its performance on the testing data is comparable to or slightly worse than the default model. Therefore, the tuning process did not lead to a significant improvement in the model's generalization ability.

**Recommendations:**

I recommend implementing the Tuned Random Forest Model for predicting Item_Outlet_Sales due to the following reasons:
  - The Tuned Random Forest Model showcases a robust training R-squared of 0.94, indicating its good fit to the training data. However, it exhibits challenges in generalizing to new data, as evidenced by the testing R-squared of 0.56.
  - I suggest using Root Mean Squared Error (RMSE). RMSE provides a measure of prediction accuracy in the same units as the target variable (Item_Outlet_Sales).
Both Random Forest models display signs of overfitting, with the Tuned model showing improved generalization capabilities.

**Limitations & Next Steps**
In conclusion, although the Tuned Random Forest model excels in training fit and RMSE for predicting Item_Outlet sales, we must remain cautious about the risk of overfitting and consider exploring further adjustments or alternative models.

**For further information**
For any additional questions, please contact email: imen.yahyaoui.codingdojo@gmail.com
