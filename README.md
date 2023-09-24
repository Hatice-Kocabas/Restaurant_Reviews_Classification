# Restaurant Review Sentiment Analysis

This project aims to predict whether restaurant reviews are positive or negative using Natural Language Processing (NLP) techniques. Two different machine learning models, Gaussian Naive Bayes and XGBoost, were trained and evaluated on a dataset of restaurant reviews.

## Dataset

The dataset used for this project is in the 'Restaurant_Reviews.tsv' file and contains restaurant reviews along with their corresponding labels (1 for positive, 0 for negative). The dataset was loaded into a Pandas DataFrame for analysis.

### Exploratory Data Analysis

- The dataset was explored to understand its structure and characteristics.
- The distribution of positive and negative reviews was visualized using a countplot.
- Basic statistics like the number of positive and negative reviews were calculated.

## Data Preprocessing

- Text preprocessing was performed on the reviews to prepare them for model training.
- Textual data was cleaned by removing non-alphabetical characters, converting text to lowercase, and tokenizing the text.
- Stop words were removed, and words were stemmed using the Porter stemming algorithm.
- The cleaned text data was stored in the 'corpus' variable.

## Feature Extraction

- Count Vectorization was used to convert the text data into numerical form.
- The 'CountVectorizer' from scikit-learn was employed with a maximum of 1500 features.
- The feature matrix 'x' and target variable 'y' were prepared.

## Model Building and Training

### Gaussian Naive Bayes

- A Gaussian Naive Bayes classifier was trained on the feature matrix 'x' and target variable 'y'.
- The dataset was split into training and testing sets using a 80/20 split.
- Model performance was evaluated using accuracy and a confusion matrix.

### XGBoost

- An XGBoost classifier was trained on the same data.
- Similar to the Naive Bayes model, the dataset was split into training and testing sets.
- Model performance was evaluated using accuracy and a confusion matrix.

## Results

- Both Gaussian Naive Bayes and XGBoost models were evaluated for their accuracy.
- XGBoost outperformed Gaussian Naive Bayes in terms of accuracy, achieving a higher prediction accuracy.

## Conclusion

This project demonstrates the application of NLP techniques to sentiment analysis of restaurant reviews. It shows that XGBoost is a suitable choice for this task, as it achieved better predictive performance compared to Gaussian Naive Bayes.

Feel free to use and modify this code for your own projects or further improvements.

If you have any questions or feedback, please don't hesitate to reach out.

**Note:** Make sure to download the required NLTK stopwords by running `nltk.download('stopwords')` before running the code.
