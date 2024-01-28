# Supervised Learning Project: Predicting Diabetes 🩺

## Project Outcomes 🎯

### Goal 🌟
- Utilize supervised learning techniques to predict whether a patient has diabetes based on diagnostic measurements. 🔍
- Enhance skills in exploratory data analysis, data preprocessing, and model evaluation using various machine learning algorithms. 📊
- ![Diabetes Analysis](https://media.giphy.com/media/lnlvaqJEhQtwMpkUzc/giphy.gif)


### Project Description 📝
- Applied supervised learning on the [Diabetes dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset) from the National Institute of Diabetes and Digestive and Kidney Diseases.
- Tasks included exploratory data analysis, data cleaning, handling missing values, feature engineering, and building predictive models. 🧬

### Conclusions 📈

#### Discussion of Results for the Training Section 📚
- Results from the Training of 3 Models:
  
  | Model                      | Cross-Validation | Hyper Parameters | Best Model Measure | Training Recall | Test Recall | Test F1 Score |
  |----------------------------|------------------|------------------|--------------------|-----------------|-------------|---------------|
  | Logistic Regression        | None             | N/A              | N/A                | N/A             | 0.67        | 0.66          |
  | Logistic Regression        | K-Folds (10 folds)| -                | Recall             | 0.643           | 0.6         | 0.706         |
  | Random Forest              | K-Folds (5 folds) | GridSearch       | Recall             | 0.588           | 0.667       | 0.727         |
  | Random Forest              | K-Folds (10 folds)| RandomizedSearch | Recall             | 0.576           | 0.6         | 0.679         |

#### Reflections on the Model Training Measures 🤔
- Findings from Model Training:
  - The basic Logistic Regression without cross-validation performed best on Test data using Recall score.
  - Random Forest with GridSearch exhibited promising results, especially in F1 score, which is a blend of Recall and Precision.
  - The Random Forest model's performance was close to Logistic Regression on Recall, despite additional efforts in hyperparameter tuning.

#### Overall Conclusions 🧐
- The plain Logistic Regression model performed unexpectedly well on Recall for Test data compared to models involving Cross-Validation and Hyperparameter Tuning.
- The Random Forest with Grid Search shows promise but may improve with:
  - More computational resources and hyperparameter tuning.
  - Experimentation with different performance metrics.
  - Implementation of feature selection methodologies and oversampling techniques.

### Next Steps 🛤️
- Areas for further exploration and learning include:
  - Understanding statistical tests for feature relations.
  - Employing feature selection methodologies and handling missing data and outliers.
  - Exploring oversampling techniques for potential model improvement.
  - Researching computational resources and optimization techniques for hyperparameter tuning.
