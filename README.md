# Fake News Detection

## 1. Introduction

The rampant spread of misinformation and fake news in the digital era necessitates robust solutions for detection. This report details the comprehensive process involved in developing an effective fake news detection model. The dataset utilized contains news articles labeled as real or fake, forming the basis for constructing, training, and evaluating the model.

## 2. Methodology

### 2.1 Data Preprocessing

#### 2.1.1 Importing Necessary Packages and Dataset
The project initiated with the importation of essential packages and the extraction of the dataset, creating the foundation for subsequent analysis.

#### 2.1.2 Checking Data Shape and Null Values
An exploration of the dataset's shape and identification of null values led to their handling by replacing them with an empty string, ensuring the integrity of the dataset.

#### 2.1.3 Concatenating Title and Author Columns
To streamline the analysis, the title and author columns were concatenated into a new column named 'content.' This step aimed to consolidate relevant information for effective feature extraction.

#### 2.1.4 Text Preprocessing with Porter Stemmer
Text data underwent meticulous preprocessing using the Porter Stemmer. This technique was applied to improve the model's understanding by standardizing word forms and eliminating unnecessary information.

### 2.2 Feature Engineering

#### 2.2.1 Transforming Text Data into Numerical Data
Feature engineering involved transforming the textual data into numerical data using the TfidfVectorizer. This step enabled the development of machine learning models based on numerical representations of the text.

## 3. Model Training and Evaluation

### 3.1 Splitting Data into Training and Testing Sets
To evaluate the model's performance accurately, the dataset was split into training and testing sets, ensuring a comprehensive assessment of the model's generalization capabilities.

### 3.2 Model Training and Evaluation
Three machine learning models—Logistic Regression, Decision Tree, and Random Forest—were selected for training and evaluation. The models were assessed based on metrics such as accuracy, precision, and F1-score to gauge their effectiveness in fake news detection.

#### 3.2.1 Logistic Regression
The Logistic Regression model demonstrated a training accuracy of 98.70%, testing accuracy of 98.32%, precision score of 97.52%, and F1-score of 98.35%.

#### 3.2.2 Decision Tree
The Decision Tree model exhibited a training accuracy of 93.58%, testing accuracy of 94.54%, precision score of 90.95%, and F1-score of 94.90%.

#### 3.2.3 Random Forest
The Random Forest model showcased exceptional performance with a training accuracy of 99.58%, testing accuracy of 99.09%, precision score of 98.89%, and F1-score of 99.08%.

### 3.3 Model Comparison

A comprehensive comparison of the model performances is presented in the following table:

| Algorithm Name       | Training Accuracy | Testing Accuracy | Precision Score | F1-Score |
|-----------------------|-------------------|------------------|------------------|----------|
| Logistic Regression   | 98.70%            | 98.32%           | 97.52%           | 98.35%   |
| Decision Tree         | 93.58%            | 94.54%           | 90.95%           | 94.90%   |
| Random Forest         | 99.58%            | 99.09%           | 98.89%           | 99.08%   |

## 4. Conclusion

The results underscore the effectiveness of all models, with each demonstrating commendable accuracy in fake news detection. Notably, the Random Forest model stands out with the highest testing accuracy, precision score, and F1-score, making it the preferred choice for fake news detection in this project. This comprehensive report provides insights into the end-to-end process of developing a robust fake news detection solution.
