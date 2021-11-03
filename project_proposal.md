# Project Proposal

For this project I intend to examine reviews from Tiktok to understand the trends of what is being highly received with the app and what is being poorly received. 
This would allow Tiktok to better structure their app and discover what within the data is being discussed to improve upon the app for a better end user experience. 
To this end, I plan on examining the problem with a sentiment analysis after performing some natural language processing on the reviews, creating unsupervised models such as clustering as the data exploration shows is possible.

## Data Used and MVP

The data for this project will come from [Kaggle](https://www.kaggle.com/shivamb/35-million-tiktok-mobile-app-reviews), which will then be restricted to 2020 and 2021 reviews as to create a model built around the most up to date app and sentiments for the app. 
The **MVP** for this project would be a topic model showing what are the most important topics and what words tend to be associated with them.
I intend to use pandas to read in and explore the data, spaCy and NLTK to perform NLP on the review data as well as scikit-Learn to model. To visualize the data I plan to use seaborn, matplotlib, and potentially Bokeh, Plotly, and Tableau depending on the circumstances that would best fit the data.
