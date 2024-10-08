# Twitter Data Sentiment Analysis using NLP - Machine Learning

## Project Overview
This project aims to perform sentiment analysis on Twitter data using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to classify tweets as either positive or negative based on their content.

![images](https://github.com/user-attachments/assets/f1acbdee-5830-40e1-be1f-62270424c81a)

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
- This usecase can be done in better way using lemmatizer , word2vec , avgword2vec , wordembeddings , and model can be developed using ensemble methods like xgboost..and use 
  deep learning techniques as well. I will improve this usecase further using those technique and welcoming everyone to do the same.
