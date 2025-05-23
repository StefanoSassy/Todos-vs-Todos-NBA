# Todos-vs-Todos-NBA

## Models and Techniques Utilized

This project focuses on predicting NBA game winners by utilizing data from players. To achieve this, various Machine Learning models were implemented and combined using an ensemble approach. Below are the key models and techniques used:

- **Logistic Regression**  
  A logistic regression model is used to estimate the probability of a team winning the game. The `predict_proba` function is employed to obtain the probability of the positive class, which is essential for subsequently combining the model's output with others.

- **Random Forest**  
  Using the `RandomForestClassifier`, this model leverages the power of multiple decision trees to capture non-linear relationships and complex patterns in the data. It helps enhance accuracy and reduce overfitting.

- **XGBoost**  
  By employing the `XGBClassifier`, a boosting approach is implemented that combines multiple weak learners to optimize predictions. XGBoost is particularly effective at detecting complex interactions among variables.

- **Ensemble (Model Combination)**  
  An ensemble approach is applied by averaging the probabilities obtained from the Logistic Regression, Random Forest, and XGBoost models. The final prediction is determined by applying a threshold (0.5) to the averaged probabilities, enhancing the overall robustness and reliability of the outcome.

Additional techniques and tools incorporated in the project include:

- **Preprocessing:**  
  The `StandardScaler` was used to normalize the features, ensuring that all variables contribute equally to the model's performance.

- **Hyperparameter Tuning:**  
  `GridSearchCV` was utilized to optimize the parameters of each model, thereby enhancing their performance.

- **Dimensionality Reduction:**  
  Principal Component Analysis (PCA) was implemented to explore data variance and reduce dimensionality when necessary.

- **Evaluation and Visualization:**  
  The project makes extensive use of performance metrics such as accuracy, ROC curves, and Precision-Recall curves (using functions like `roc_curve`, `roc_auc_score`, and `precision_recall_curve`) to evaluate model performance. Moreover, `matplotlib` is leveraged to create a wide range of visualizations, which aid in understanding the data distributions, model comparisons, and overall insights.

This comprehensive combination of models and techniques allows for a robust comparison of different approaches and harnesses their respective strengths to predict game outcomes effectively, while also providing rich visual insights to support the decision-making process.
