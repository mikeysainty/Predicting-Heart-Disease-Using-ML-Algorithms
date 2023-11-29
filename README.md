# Predicting_Heart_Disease_Using_ML_Algorithms

## Purpose
This project aims to harness the power of machine learning (ML) algorithms to predict heart disease using the 2015 heart disease data from the Behavioral Risk Factor Surveillance System (BRFSS), available on [Kaggle](https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system). We conducted an in-depth analysis to understand the accuracy of different ML algorithms in predicting heart disease and to identify the most influential factors. The study addresses key research questions about population generalizations, statistically significant factors in determining heart disease, and the optimal minimal factors for accurate predictions.

## Methodology
We employed various machine learning algorithms, including Logistic Regression, Decision Trees, Random Forest, and Naive Bayes, to analyze the dataset. These algorithms were chosen for their diverse approaches in handling classification problems and their ability to provide insights into feature importance.

## Dataset Features
The dataset features critical health indicators and demographics, such as high blood pressure, cholesterol levels, smoking status, diabetes, physical activity, dietary habits, alcohol consumption, healthcare access, mental and physical health, mobility difficulties, along with personal demographics like sex, age, education, and income.

## Key Research Questions
- What generalizations can we make about the surveyed population, and how do these influence the results?
- Which factors are statistically significant in determining heart disease?
- What are the non-significant factors?
- What is the minimal set of factors required for reasonable heart disease prediction?
- Which ML model performs best for this dataset, and what might be the reasons for its performance?

## Target Audience
Our research is particularly beneficial for healthcare facilities, medical professionals, researchers, public policy makers, and anyone involved in the healthcare field, providing them with insights into the predictive power of ML in diagnosing heart disease.

## Analysis and Findings

- **Logistic Regression**: 
  - Identified stroke history, gender (males more prone), high blood pressure, high cholesterol, and poor general health as significant risk factors for heart disease.
  - Difficulty in climbing stairs was also significant but may be a symptom of other risk factors.

- **Decision Trees**: 
  - Highlighted high blood pressure and high cholesterol as key predictors.
  - Healthcare-related attributes were less significant in direct risk but important in treatment and prevention strategies.

- **Random Forest**: 
  - Achieved an accuracy of 90%, with the confusion matrix showing a substantial number of true positives.
  - Effectiveness of identified risk factors in predicting heart disease was underscored.

- **Model Comparison**: 
  - Logistic regression was most effective, with an accuracy of 90.9%.
  - Random Forest followed closely, while the SVM model showed limitations in classifying positive cases despite high accuracy.

## Conclusion

The study concludes that:
- Strokes, being male, high cholesterol, high blood pressure, and poor physical health are crucial in predicting heart disease.
- The accuracy of logistic regression highlights the importance of focusing on these variables in heart disease risk assessment.
- Mental health, while not directly significant, may indirectly affect heart disease, suggesting an area for future research.
- Emphasizing physical health maintenance is essential in minimizing heart disease risk.

## Limitations and Improvements

- The use of categorical data may limit model accuracy.
- More detailed, numerical data could improve predictions.
- Expanding the dataset to include additional variables and exploring congenital vs. environmental causes of heart disease could provide richer insights.
- Utilizing the full dataset with 400,000 rows could offer a more comprehensive understanding but requires extensive data cleaning and thoughtful representation of categorical data.

## Recommendations

- Individuals with stroke history or risk factors like high cholesterol and blood pressure should actively manage these conditions.
- Consistent health maintenance is crucial for both preventing heart disease and managing it in diagnosed individuals.
- Future studies could benefit from more granular data collection, such as continuous variables or broader categorical scales for sensitive topics, to provide deeper insights.
