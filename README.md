# Diabetes Prediction Project

![Diabetes Banner](https://pharmaceuticalintelligence.com/wp-content/uploads/2021/05/machine-learning-in-healthcare-1-768x402-1.jpg) <!-- Replace with the URL of your banner image -->

## Overview

This project aims to predict the likelihood of diabetes in patients using machine learning techniques. The dataset used for this project is a collection of various health metrics, and the goal is to build a predictive model that can accurately classify individuals as either diabetic or non-diabetic.

## Dataset

The dataset used in this project is a CSV file containing medical data related to diabetes. The data includes the following features:

- **Pregnancies**: Number of pregnancies
- **Glucose**: Plasma glucose concentration
- **BloodPressure**: Diastolic blood pressure
- **SkinThickness**: Triceps skin fold thickness
- **Insulin**: 2-Hour serum insulin
- **BMI**: Body Mass Index
- **DiabetesPedigreeFunction**: Diabetes pedigree function
- **Age**: Age of the patient
- **Outcome**: Target variable (0 for non-diabetic, 1 for diabetic)

## Data Collection and Analysis

1. **Loading the Dataset**:
   The dataset is loaded into a Pandas DataFrame and initial inspection reveals 768 rows and 9 columns.

2. **Descriptive Statistics**:
   Statistical measures provide insights into the dataset, including mean, standard deviation, minimum, and maximum values for each feature.

3. **Data Distribution**:
   The dataset is analyzed to determine the number of diabetic (268) and non-diabetic (500) patients. Mean values are computed for each feature, grouped by the outcome.

## Data Preprocessing

1. **Feature and Target Variables**:
   - **Features (X)**: All columns except 'Outcome'.
   - **Target (Y)**: The 'Outcome' column.

2. **Standardization**:
   The feature data is standardized using `StandardScaler` to ensure that all features have a similar scale.

3. **Data Splitting**:
   The dataset is split into training and testing sets with 80% of the data used for training and 20% for testing.

## Model Building and Evaluation

1. **Model Selection**:
   A Support Vector Machine (SVM) with a linear kernel is used for classification.

2. **Training**:
   The model is trained using the training dataset.

3. **Evaluation**:
   - **Training Accuracy**: 78.66%
   - **Testing Accuracy**: 77.27%

The model demonstrates a good performance in predicting diabetes with reasonably high accuracy on both training and testing datasets.

## Conclusion

This project showcases the process of building a machine learning model to predict diabetes based on various health metrics. The results indicate that the model can effectively classify patients as diabetic or non-diabetic, with a notable level of accuracy.

## Future Work

Future improvements may include exploring other machine learning algorithms, feature engineering, and hyperparameter tuning to enhance model performance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

Special thanks data providers who made this project possible.
