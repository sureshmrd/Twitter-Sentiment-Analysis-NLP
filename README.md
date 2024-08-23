# Twitter Data Sentiment Analysis using NLP - Machine Learning

## Project Overview
This project aims to perform sentiment analysis on Twitter data using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to classify tweets as either positive or negative based on their content.

https://www.google.com/imgres?q=twitter%20sentiment%20analysis%20using%20ml&imgurl=https%3A%2F%2Fwww.aimtechnologies.co%2Fwp-content%2Fuploads%2F2024%2F01%2FTwitter-Sentiment-Analysis.png&imgrefurl=https%3A%2F%2Fwww.aimtechnologies.co%2F2024%2F01%2F09%2Ftwitter-sentiment-analysis-decoding-the-social-media-pulse%2F&docid=vlzwIVHIGtoEbM&tbnid=EbSpekFpY3yb2M&vet=12ahUKEwjNzZiAy4qIAxUvTGwGHUW0Ai4QM3oECHwQAA..i&w=1040&h=508&hcb=2&ved=2ahUKEwjNzZiAy4qIAxUvTGwGHUW0Ai4QM3oECHwQAA

## Dataset
The dataset used for this project is **Sentiment140**, obtained from Kaggle. It contains 1.6 million textual data points with the following columns:
- `target`: The sentiment of the tweet (0 = negative, 4 = positive)
- `ids`: The unique ID of the tweet
- `date`: The date and time of the tweet
- `flag`: The query (if any)
- `user`: The user who tweeted
- `text`: The text content of the tweet

## Preprocessing
The following preprocessing steps were applied to the dataset:
- **Stopwords Removal**: Removed common English stopwords using `stopwords('english')`.
- **Stemming**: Applied stemming to reduce words to their base form using `PorterStemmer()`.
- **TF-IDF Transformation**: Transformed the textual data into numerical features using `TfidfVectorizer()`.

## Model Training
- **Algorithm**: Logistic Regression
- The processed data was used to train a logistic regression model.
- The output labels were binary (0 and 1), where:
  - `0` indicates a negative tweet.
  - `1` indicates a positive tweet.

## Model Saving
- The trained model was saved using the `pickle` library for future use and deployment.

## Result
- The logistic regression model achieved good performance on the test data, accurately classifying tweets as positive or 
  negative.

## Conclusion
- This project demonstrates the application of NLP and Machine Learning for sentiment analysis on Twitter data. The trained 
  model can be used to analyze and classify tweets based on their sentiment.
