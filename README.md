# Recipe Traffic Prediction
Recipe Traffic Prediction is a machine learning project that aims to develop a model for accurately predicting the traffic levels of recipes. By analyzing various recipe features, such as calories, carbohydrates, protein, and more, the model can identify which recipes are likely to attract high traffic. This information can help businesses optimize their marketing strategies and drive sales and profit. The project also addresses the challenge of imbalanced data using the SMOTETomek technique.

## Aim
The aim of this project is to develop a machine learning model that can accurately predict the traffic levels of recipes. By understanding which recipes are likely to attract high traffic, businesses can optimize their marketing strategies, increase user engagement, and drive sales and profit.

## Data
The dataset used for this project consists of various features related to recipes, including calories, carbohydrate content, sugar content, protein content, recipe category, number of servings, and a label indicating whether the recipe is associated with high traffic. The dataset was collected from a popular recipe website and contains a mix of high-traffic and low-traffic recipes.

## Handling Data Imbalance
The original dataset is imbalanced, with a significantly higher number of low-traffic recipes compared to high-traffic recipes. To address this issue, the SMOTETomek technique was employed to handle data imbalance. SMOTETomek combines the benefits of oversampling (SMOTE) and undersampling (Tomek Links). This approach helps to increase the representation of the minority class (high-traffic recipes) while removing ambiguous instances, resulting in a more balanced and better-separated dataset. Handling data imbalance is crucial to improve the performance of machine learning models when dealing with imbalanced data.

## Model Design
Two machine learning models were considered for the recipe traffic prediction task: Support Vector Classifier (SVC) and Random Forest Classifier.

The SVC algorithm was chosen as the primary model for its ability to handle non-linear decision boundaries and effectively classify data. It was trained on the preprocessed dataset to learn the patterns and relationships between recipe features and their corresponding traffic levels.

Additionally, a Random Forest Classifier was built as a baseline model for comparison. Random Forest is an ensemble learning method that combines multiple decision trees to make predictions. It was trained on the same preprocessed dataset to evaluate its performance in predicting recipe traffic.

Both models were evaluated based on their accuracy, precision, recall, and F1-scores to determine their effectiveness in predicting high-traffic recipes.

## Model Results
The tuned SVC model achieved higher accuracy (85%) than the Random Forest base model (82%), indicating its competence in predicting high-traffic recipes accurately.

The SVC model showed excellent performance in classifying high-traffic recipes, with precision, recall, and F1-scores of 0.83, capturing 83% of actual high-traffic recipes. In comparison, the Random Forest model achieved lower precision, recall, and F1-scores of 0.82 and 0.79 respectively.

With an overall accuracy of 84% on the test dataset, the tuned SVC model outperformed the Random Forest model (82%) in correctly classifying recipes, highlighting its potential to drive sales and profit by accurately predicting high-traffic recipes.

## Possible Modifications/Improvements
Model Hyperparameter Tuning: Conduct a more comprehensive hyperparameter search to optimize the performance of both models.

Ensemble Methods: Implement ensemble methods, such as stacking or boosting, to combine the predictions of multiple models and potentially improve overall performance.

Regular Monitoring and Updating: Regularly monitor the model's performance and retrain it with updated data to ensure its accuracy and relevance in a changing recipe landscape.

Please refer to the provided code and documentation for more detailed implementation and usage instructions.
