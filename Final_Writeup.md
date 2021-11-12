# Understanding TikTok

Alex Stake

## Abstract

The goal of this project was to examine reviews of the video streaming app TikTok to analyze sentiment and discover what people discuss in the reviews. 
The data came from a Kaggle dataset that covers 3.5 million reviews from 2015 through 2021. I performed NLP through spacy to tokenize the data and then I explored multiple topic models including LSA, NMF, LDA, and CoRex to discover what topics were being discussed and whether the sentiment was primarily positive or negative. 
This goal was best achieved through a CoRex topic model, discovering 4 major topics centered on True Reviews, Requests, Positive Sentiment, and Content that is enjoyed by users.

## Design

For this project I examined reviews from Tiktok to understand the trends of what is being highly received with the app and what is being poorly received. This would allow Tiktok to better structure their app and discover what within the data is being discussed to improve upon the app for a better end user experience. To this end, I examined the problem with a sentiment analysis after performing some natural language processing on the reviews, creating a topic model to show what users are talking about in reviews.

## Data

The data set comes from [Kaggle](https://www.kaggle.com/shivamb/35-million-tiktok-mobile-app-reviews) and consists of 3.5 million reviews of TikTok from 2015 to 2021.
After narrowing the data down to only the most recent reviews from 2020 and 2021 there were 1.9 million reviews. An observation in this dataset consists of a review, the unique ID of the review, the number of upvotes a review received, the app version, and the date the review was posted from. 

## Algorithms
*NLP*

Data was tokenized through spacy after ingestion through pandas, with stop words including words relating directly to TikTok and app as well as most English stop words.
In addition to standard tokenization of the data, I built a vectorizer that used bi-grams to see if there would be more clear topics in the higher performing models.

*Models*

After data was tokenized, I built several models, starting with LSA and NMF and eventually performing topic modeling with LDA and CoRex. After building all models, I settled on using CoRex with bi-grams for the final model as it had the most clear topics. 
I built the model around 4 topics as it explained the most data with the least overlap. These topics were True Reviews, Requests, Positive Sentiment, and Content. Even so, there was a high amount of overlap in topic 1 and topics 3 and 4 in their highest words.

## Tools
- Pandas and Numpy for data manipulation and ingestion
- Spacy and CoRex for Natural Language Processing
- Scikit-Learn and CoRex for topic modeling
- Matplotlib and Seaborn for plotting and visualization

## Communication

The data is presented through the [slides](https://github.com/ajstake/Unsupervised_Tik_Tok/blob/main/Tiktok_Unsupervised_Presentation.pdf) and [figures](https://github.com/ajstake/Unsupervised_Tik_Tok/tree/main/figures) provided.
