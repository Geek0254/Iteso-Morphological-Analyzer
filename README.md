# Iteso-Morphological-Analyzer

This repository contains a morphological analyzer model for the Teso language. It is built using scikit-learn, a popular machine learning library in Python.

## Dataset

The model is trained on the Teso Corpus Dataset, which consists of labeled Teso words and their corresponding part-of-speech tags. The dataset is loaded using the pandas library.

## Model Training

The model is trained using logistic regression, a widely used classification algorithm. The training data is split into train and test sets using the `train_test_split` function from scikit-learn. 
The input features (Teso words) are transformed into numerical vectors using the `CountVectorizer` class, which converts text into a matrix of token counts. 
The transformed data is then used to train the logistic regression model.

## Model Evaluation

After training the model, it is evaluated using various performance metrics such as accuracy, precision, recall, and F1 score. 
These metrics are calculated using the test set and the predictions made by the model.

Additionally, a confusion matrix is plotted using the `confusion_matrix` function from scikit-learn and visualized using the seaborn and matplotlib libraries.

## Usage

To use the model, you can enter a word and check if it is classified as an Iteso word. 
The input word is transformed using the trained vectorizer, and the model predicts its class. The result is then printed on the console.

Please note that in order to run the code and use the model, you need to have the required libraries installed and provide the path to the Teso Corpus Dataset CSV file.

## How to Run

1. Clone the repository to your local machine.
2. Install the required libraries mentioned in the code (pandas, scikit-learn, matplotlib, seaborn).
3. Provide the path to the Teso Corpus Dataset CSV file in the code or alternatively save the csv in the same directory as your .ipynb file.
4. Run the script, and it will train the model, evaluate its performance, and prompt you to enter a word for classification.

Feel free to modify the code and experiment with different models, feature engineering techniques, or datasets to improve the performance of the morphological analyzer.

