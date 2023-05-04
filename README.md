# Sentiment Analysis of Yelp Reviews Using BERT
This project uses the BERT-based model for sentiment analysis of Yelp reviews. The model was trained on a large multilingual corpus and is able to provide a sentiment score ranging from 1 to 5, where 1 represents the most negative sentiment and 5 represents the most positive sentiment.

## Installation and Dependencies

Navigate to the project directory and install the required packages using the following command:
```
pip install -r requirements.txt
```
This project requires the following dependencies:
- Transformers
- PyTorch
- Requests
- BeautifulSoup
- Pandas
- NumPy

## Steps
The project involves the following steps:

1. Install and import the necessary dependencies.
2. Instantiate the BERT-based model for sentiment analysis.
3. Encode and calculate the sentiment score for a sample review.
4. Collect Yelp reviews by web scraping the website using BeautifulSoup.
5. Load the collected reviews into a Pandas DataFrame and calculate the sentiment score for each review using the BERT-based model.
6. Compute the overall sentiment score of the reviews.
7. The sentiment_score function takes in a review as input and returns its sentiment score using the pre-trained BERT-based model. The truncation=True parameter is added to the tokenizer.encode() method to truncate the input sequence to the maximum length allowed by the model.

The Yelp reviews are loaded into a Pandas DataFrame with a column named review. The apply method is used to apply the sentiment_score function to each review in the DataFrame and compute its sentiment score. The overall sentiment score is computed by taking the mean of all the sentiment scores in the DataFrame.

## Conclusion
This project demonstrates the use of a pre-trained BERT-based model for sentiment analysis of Yelp reviews. The model provides a robust and accurate way to evaluate the sentiment of large volumes of text data.
