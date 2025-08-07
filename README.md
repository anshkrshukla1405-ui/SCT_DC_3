# SCT_DC_3
# Bank Marketing Prediction Using Decision Tree Classifier

## About This Project

This project focuses on predicting whether a bank customer will subscribe to a marketing campaign using a Decision Tree model. The goal is to assist banks in identifying potential customers who are more likely to say "yes" to the offer, thereby improving targeting efficiency.

The dataset used contains real-world customer data with both demographic and marketing-related features.

## Dataset Summary

- Contains about 45,000 records.
- Features include age, job type, marital status, education, contact information, past campaign results, and more.
- The target variable is a binary label indicating subscription status (yes/no).
- The data has both numerical and categorical features, with class imbalance (fewer subscribers than non-subscribers).

## Steps Taken

1. **Loading and Exploring Data**  
   Used pandas to load the data, then examined structure, types, and summary statistics to understand the dataset.

2. **Preprocessing**  
   - Converted the target into 0/1 values (`no` → 0, `yes` → 1).  
   - Applied one-hot encoding to categorical variables to convert them into numeric format for the model.

3. **Splitting Data**  
   Divided the data into training and testing sets (80%/20%) to enable unbiased model evaluation.

4. **Training the Model**  
   Built and trained a Decision Tree classifier with default settings and ensured reproducibility using a fixed random seed.

5. **Evaluating Performance**  
   Measured model accuracy and reviewed precision, recall, and F1-score, especially because the dataset is unbalanced.  
   The evaluation helped understand strengths and weaknesses of the model for predicting each class.

6. **Visualizing the Model**  
   Created a decision tree plot to make the model interpretable and to highlight the most important features influencing decisions.

## Key Findings

- The model achieved about 87% accuracy, which means it correctly predicted customer behavior in most cases.
- Prediction works better for the majority class (customers who did not subscribe) due to imbalanced data.
- Important factors affecting predictions included call duration, how the contact was made, and previous campaign outcomes.
- Visualization makes it easier to explain the model to non-technical stakeholders.

## Technologies Used

- Python programming language
- pandas for data manipulation
- scikit-learn for modeling and evaluation
- matplotlib for visualization
- Jupyter Notebook as the development environment

## How to Use This Project

1. Download or clone the repository.
2. Ensure Python and the required libraries (`pandas`, `scikit-learn`, `matplotlib`) are installed.
3. Run the Jupyter Notebook stepwise to load data, preprocess it, train the model, evaluate results, and visualize the tree.

## What I Learned

- The importance of correctly encoding categorical variables for machine learning models.
- How to handle imbalanced classification problems and why multiple metrics besides accuracy matter.
- Building interpretable machine learning models and visualizing decision trees.
- The value of a methodical approach: data loading, preprocessing, splitting, training, evaluation, and interpretation.
