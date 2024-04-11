Prediction of Product Sales

Author: Imen YAHYAOUI

Business problem:
make predictions about future sales.

Data:
The dataset contains information about products, including their IDs, weights, fat content, visibility in stores, category, and retail prices. It also includes store details like IDs, establishment years, sizes, location types, and types (grocery or supermarket). The target variable is the sales of each product in a specific store. This dataset is valuable for retail analysis and predictive modeling tasks.
The Data used: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

Methods
Data preparation steps with explanation and justification for choices

Handling Missing Values:
Missing data can disrupt model training. Impute missing values using median for numerical features,most frequent category for ordinal features, and fill value Missing for categorical features.

Encoding Categorical Variables:
Convert categorical variables into numerical format for machine learning algorithms. Use one-hot encoding for nominal variables and label encoding for ordinal variables.

Feature Scaling:
Normalize feature scales to prevent bias in models sensitive to scale differences. Apply standardization (mean = 0, standard deviation = 1)based on data distribution and algorithm requirements.

Results






La figure montre une visualisation de la façon dont les différents types de magasins (Outlet_Type) sont liés aux ventes de produits dans ces magasins (Item_Outlet_Sales), ce qui peut aider à identifier des tendances ou des modèles significatifs dans les données.

Visual 2 Title
Model
Describe your final model

Report the most important metrics

Refer to the metrics to describe how well the model would solve the business problem

Recommendations:
More of your own text here

Limitations & Next Steps
More of your own text here

For further information
For any additional questions, please contact email
