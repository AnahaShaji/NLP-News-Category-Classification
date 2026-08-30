# NLP-Based News Category Classification

## Project Overview

This project uses Natural Language Processing (NLP) and Machine Learning to automatically classify news articles into different categories.

The system classifies news articles into five categories:

- Business
- Entertainment
- Politics
- Sport
- Tech

## Dataset

The project uses the BBC News dataset.

- **Total Articles:** 2,225
- **Categories:** 5
- **Dataset Source:** Derek Greene – BBC Datasets
- **Training Articles:** 1,780
- **Testing Articles:** 445

## Technologies Used

- Python
- Pandas
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn

## Methodology

The project follows these steps:

1. Load the BBC News dataset.
2. Preprocess the news articles.
3. Split the dataset into training and testing data.
4. Convert the cleaned text into numerical features using TF-IDF.
5. Train a Multinomial Naive Bayes classifier.
6. Predict the categories of test articles.
7. Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.
8. Test the model with a new news article.

## Text Preprocessing

The following preprocessing steps are performed:

- Convert text to lowercase
- Remove punctuation and numbers
- Split the text into words
- Remove English stopwords

## Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert the cleaned news articles into numerical features.

The TF-IDF vectorizer uses a maximum of **5,000 features** for representing the news articles.

## Model

The project uses the **Multinomial Naive Bayes** algorithm for news category classification.

The model is trained using the TF-IDF features extracted from the training articles.

## Model Evaluation

The trained model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Results

The model achieved an overall accuracy of **98.43%** on the test dataset.

- **Test Articles:** 445
- **Correct Predictions:** 438
- **Incorrect Predictions:** 7
- **Accuracy:** 98.43%

The model performed well across all five news categories.

### Classification Performance

| Category | Precision | Recall | F1-Score |
|----------|-----------|--------|----------|
| Business | 0.99 | 0.99 | 0.99 |
| Entertainment | 1.00 | 0.97 | 0.99 |
| Politics | 0.97 | 1.00 | 0.98 |
| Sport | 0.97 | 1.00 | 0.99 |
| Tech | 1.00 | 0.95 | 0.97 |

The classification results show that the model provides high precision, recall, and F1-scores for all five categories.

## Sample Prediction

The trained model was also tested with a new news article related to football.

The model successfully predicted the category as:

**Sport**

## Project Structure

```text
NLP-News-Category-Classification/
│
├── NLP_News_Category_Classification.ipynb
└── README.md
```

## How to Run

1. Download or clone this repository.
2. Open the `.ipynb` notebook using Google Colab or Jupyter Notebook.
3. Download the BBC News dataset from the original source.
4. Extract the dataset into the required folder.
5. Run the notebook cells in order.

## Dataset Source

Derek Greene – BBC Datasets

https://derekgreene.com/bbc/

## Conclusion

This project demonstrates how Natural Language Processing and Machine Learning can be used to automatically classify news articles into different categories.

The Multinomial Naive Bayes model, combined with TF-IDF feature extraction, achieved **98.43% accuracy** on the test dataset. The results show that the model can effectively distinguish between Business, Entertainment, Politics, Sport, and Tech news articles.
