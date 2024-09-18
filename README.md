# 🌍 Satellite Land Cover Classification with Random Forest 🌲🌾

   ## Overview
Welcome to the Satellite Land Cover Classification project! 🎉 This repository features a Random Forest Classifier trained on Sentinel-2 satellite data to classify different land cover types (think forests, fields, and water bodies) using various experiments with satellite image features. 🌍🛰️

Here, you’ll find experiments where I test different combinations of texture features, vegetation indices, spectral bands, and terrain data to see which ones work best for classifying land cover. We also use SHAP to explain the model and Permutation Importance to see which features matter. Ready to dive in? Let’s go! 🚀

What You’ll Find Inside
Key Components:
Data Preprocessing:
The input data is loaded from a CSV file (All_features_input_sentinel2_train.csv). It’s essential to separate the features (X) from the target class (y) for training.

##  ⚠️ Important: Both the training and validation datasets need to be in CSV format. Ensure your CSV has all the features you plan to use and the target variable (classid). 🎯

Feature Selection Experiments:
I run four experiments using different combinations of features:
Texture features (like contrast and variance)
Vegetation indices (like NDVI, SAVI)
Spectral bands (specific Sentinel-2 bands)
Terrain features (like slope and elevation) Each experiment brings its insights! 🔍

Model Training with Random Forest:
For each experiment, I split the data into training and testing sets.
We use GridSearchCV to tune the hyperparameters (like number of trees and depth) and find the best Random Forest model. 🌳🔧
Cross-validation checks how well the model performs across different data splits.
Results & Model Evaluation:

After training, we evaluate the model on test data using:
Accuracy scores 🏆
Classification report 📊
Confusion matrix 🤔

Feature Importance & Explainability:
SHAP values are used to explain the model predictions—why did it predict this class? 🔮
We also check Permutation Importance to see how important each feature is by randomly shuffling them and observing the impact.
Visuals, Visuals, Visuals! 🎨

Bar plots for feature importance
Confusion matrices to show how well the model performed
SHAP summary plots to explain the model’s decisions visually
Ready for some stunning visuals? 😎


# How to Run
1. pip install pandas numpy scikit-learn matplotlib seab

2. Place your CSV file (`All_features_input_sentinel2_train.csv`) in the same directory as the script.

3. Run the script! It will automatically:
- Process each experiment.
- Train the model.
- Evaluate performance.
- Generate and display beautiful visualizations of feature importance, confusion matrices, and SHAP plots.

4. Check the console for:
- Best model parameters 💡
- Accuracy scores 🏅
- Feature importance rankings 🔝

## Results and Insights

- **Feature Importance:** Know which satellite features are the real MVPs! 🏆
- **Confusion Matrix:** See how well the model is predicting each class.
- **SHAP Values:** Get an intuitive understanding of how each feature contributes to the final prediction. 💬
- **Permutation Importance:** Just how essential is each feature? Find out by shuffling! 🎲

## Have Fun! 🎉
Happy coding! 💻🌍


# Results snippet
Model Evaluation report for experiment 1
![image](https://github.com/user-attachments/assets/8fc201d9-0660-4dd8-b47d-25eb75f22905)

![image](https://github.com/user-attachments/assets/9d4ab2a5-4d3e-4fbf-a358-824250a81d9c)
![image](https://github.com/user-attachments/assets/19a7a4a1-dcac-49db-9610-5d28b2c71daa)
![image](https://github.com/user-attachments/assets/3ca05dcc-6983-4b62-bec1-f91d7601a477)
![image](https://github.com/user-attachments/assets/d4f0625e-a46e-44e6-9ead-930f2c34483f) 




