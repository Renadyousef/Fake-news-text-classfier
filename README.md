# Fake-news-text-classfier
A machine learning project to classify news articles as real or fake based on their text content, using feature engineering, TF-IDF vectorization, and logistic regression.

1.Dataset

The dataset is available on Kaggle: Fake News Classification

It contains 72,134 news articles: 35,028 real and 37,106 fake.

Columns in the dataset:

title: headline of the news article

text: full content of the news article

label: 0 = fake, 1 = real

2. Features Used

In addition to the raw text, the following features were engineered to improve model performance:

Readability (Flesch reading ease score)

Repeated punctuation (like !!, ??)

Title length

Text length

All-caps count & ratio in the title

3. Preprocessing

Text was vectorized using TF-IDF, preserving capitalization and punctuation.

Numeric features were scaled to allow negative and positive values.

Combined text vectors and numeric features to train the model.

4. Model

Logistic Regression was used as the main classifier.

Initially, with only raw text, accuracy was around 50% (random).

After feature engineering and scaling, the model reached ~96.5% accuracy.

5. Results

Balanced performance for both classes (real and fake news).

High F1-score demonstrates effective fake news detection.

Feature engineering was key to improving predictive performance

