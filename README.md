# Predicting_Heart_Disease_Using_ML_Algorithms

## Purpose
This project aims to harness the power of machine learning (ML) algorithms to predict heart disease using the 2015 heart disease data from the Behavioral Risk Factor Surveillance System (BRFSS), available on [Kaggle](https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system). We conducted an in-depth analysis to understand the accuracy of different ML algorithms in predicting heart disease and to identify the most influential factors. The study addresses key research questions about population generalizations, statistically significant factors in determining heart disease, and the optimal minimal factors for accurate predictions.

## Methodology
We employed various machine learning algorithms, including Logistic Regression, Decision Trees, Random Forest, and Naive Bayes, to analyze the dataset. These algorithms were chosen for their diverse approaches in handling classification problems and their ability to provide insights into feature importance.

## Dataset Features
The dataset features critical health indicators and demographics, such as high blood pressure, cholesterol levels, smoking status, diabetes, physical activity, dietary habits, alcohol consumption, healthcare access, mental and physical health, mobility difficulties, along with personal demographics like sex, age, education, and income.
<p align="center">
  <img width="674" alt="Dataset Features" src="https://github.com/mikeysainty/Predicting-Heart-Disease-Using-ML-Algorithms/assets/42102504/6f3f25f4-3974-483f-bc5d-174bee048bb9">
</p>

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
  - High Accuracy: Exhibited an accuracy of 90.86%, indicating strong overall predictive performance.
  - Low Recall: Demonstrated a low recall rate of 13.22%, suggesting it may miss a significant number of true positive cases (heart disease patients).
  - Significant Variables: Analysis of coefficients and p-values indicated which health indicators are significant predictors in the model.
<p align="center">
  <img width="411" alt="Logistic Regression Results" src="https://github.com/mikeysainty/Predicting-Heart-Disease-Using-ML-Algorithms/assets/42102504/5a691d77-7f09-4b59-9790-ff2239d0cc71">
</p>

- **Decision Trees**: 
  - Moderate Accuracy: Achieved an accuracy of 85.18%, which is lower than Logistic Regression and Random Forest.
  - Balanced Precision-Recall: More balanced precision (24.59%) and recall (28.49%) compared to other models, indicating a fair trade-off between false positives and false negatives.
  - Varied Performance: Performance can vary greatly depending on the complexity of the tree and the depth of the nodes.
<p align="center">
  <img width="310" alt="Decision Tree Results" src="https://github.com/mikeysainty/Predicting-Heart-Disease-Using-ML-Algorithms/assets/42102504/8d0b17f7-beff-4a1d-93b5-355de900e5ca">
</p>

- **Random Forest**: 
  - High Accuracy with Low Recall: Similar to Logistic Regression, it had high accuracy (90.40%) but suffered from low recall (11.72%).
  - Robust Against Overfitting: Generally more robust against overfitting compared to a single Decision Tree due to ensemble learning.
  - Complex Model: Involves multiple decision trees, making the model more complex and potentially harder to interpret.
<p align="center">
  <img width="297" alt="Random Forest Results" src="https://github.com/mikeysainty/Predicting-Heart-Disease-Using-ML-Algorithms/assets/42102504/a5768673-04a4-4c23-baa8-644715837028">
</p>

- **Naïve Bayes**:
  - High Recall: Exhibited the highest recall (54.43%) among the models, indicating better identification of positive cases.
  - Lower Accuracy: Lower accuracy (81.86%) compared to other models, with a higher rate of false positives.
  - Fast and Efficient: Known for its simplicity and efficiency, particularly in large datasets.
<p align="center">
  <img width="295" alt="Naive Bayes Results" src="https://github.com/mikeysainty/Predicting-Heart-Disease-Using-ML-Algorithms/assets/42102504/c0b87250-25d7-4703-89e2-dc8165c368fe"> </p>

- **Model Comparison**: 
  - **Accuracy vs Recall Trade-off**: Logistic Regression and Random Forest models demonstrate high accuracy, making them suitable for applications where overall correctness is crucial. However, they have lower recall, which could be a drawback in scenarios where identifying all positive cases (like in medical diagnostics) is essential. In contrast, Naive Bayes, with its higher recall but lower accuracy, excels in identifying positive cases but at the cost of more false positives.
  - **Complexity and Interpretability**: Decision Trees offer a balance between accuracy and recall and are relatively easy to interpret, but their performance can vary significantly. Random Forests, while more robust against overfitting than single Decision Trees, increase complexity and reduce interpretability due to their ensemble nature. Logistic Regression, on the other hand, provides a good balance between performance and interpretability.
  - **Computational Efficiency**: Naive Bayes stands out for its computational efficiency, especially in large datasets. This makes it a practical choice for applications requiring fast processing times, despite its limitations in terms of accuracy.
  - **Application Specificity**: The choice between these models is highly dependent on the specific requirements of the application. For instance, in medical diagnostics, missing a positive case (low recall) could be more detrimental than incorrectly identifying a negative case as positive (low precision).
  - **Model Robustness**: Random Forests are generally more robust against overfitting compared to Decision Trees due to their ensemble approach. However, this robustness comes at the cost of increased computational resources and complexity.

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
