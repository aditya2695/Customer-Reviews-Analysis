# Customer-Reviews-Analysis

## Introduction
<p>

This project aims to identify the main topics behind the negative reviews of British Airways using webscraping, sentiment analysis, and topic modeling techniques. We have used Python programming language to extract customer reviews of British Airways from the Airline Quality website using web scraping techniques. Then we have performed sentiment analysis on these reviews to identify the negative ones. Finally, we have used BERTopic library to cluster these negative reviews into different topics.


</p>

## Dataset

Dataset

The dataset for this project was obtained by scraping customer reviews for British Airways from the Airline Quality website. We collected reviews  resulting in a dataset of approximately 10,000 reviews.

To label the reviews as positive or negative, we used the Hugging Face sentiment predictor. This is a pre-trained NLP model that can predict the sentiment of a text as either positive or negative. We used this model to label the reviews as positive or negative based on the predicted sentiment score.

After labeling the reviews, we found that approximately 74% of them were negative. We then used topic modeling techniques to identify the main topics for the negative reviews. For this, we used the BERTopic package, which is an extension of the Latent Dirichlet Allocation (LDA) algorithm that uses BERT embeddings to represent the documents.

## Libraries Used

    BeautifulSoup4: to extract data from HTML and XML files
    Pandas: to work with data in a tabular form
    NLTK: to perform natural language processing tasks such as tokenization and stopword removal
    TextBlob: to perform sentiment analysis on the reviews
    BERTopic: to perform topic modeling on the negative reviews
    Matplotlib and Seaborn: to visualize the results

## EDA

<h3>Sentiment Distribution of British Airways Customer Reviews</h3>

<img src="images/sentiments.png" width="600">

<h3>Frequency distribution of the different words </h3>

<img src="images/frequencies.png" width="600">

## Modelling

After obtaining the negative reviews from the dataset using sentiment analysis, the next step was to perform topic modeling on these reviews to identify the main issues or topics that customers were complaining about.

We used the BERTopic package, which is based on the transformer model BERT, to perform topic modeling. BERTopic has the advantage of being very fast and efficient compared to other topic modeling algorithms, making it a great choice for large datasets.

First, we created a BERTopic model and then used it to extract the top 20 topics from the negative reviews. We visualized the topics using the pyLDAvis library, which is a popular visualization tool for topic modeling.

The resulting topics provided valuable insights into the main issues that customers were complaining about. Some of the main topics included flight delays, poor customer service, uncomfortable seats, and issues with baggage handling. By identifying these topics, the airline could focus on addressing these specific issues and improving the overall customer experience.

Overall, topic modeling proved to be a useful technique for analyzing the negative reviews and identifying the main topics of customer complaints. By using BERTopic, we were able to perform this analysis quickly and efficiently, providing the airline with valuable insights into areas for improvement.

## Conclusion

This project has shown how webscraping, sentiment analysis, and topic modeling can be used to extract insights from customer reviews. By applying these techniques to negative reviews of British Airways, we were able to identify the main topics behind the negative feedback. These insights can be used by the airline to improve its customer service and overall customer experience.