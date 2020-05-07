

# Introduction
Natural Language Processing is a Machine Learning method used to teach computers how to understand natural human language. It is not an easy task to teach these languages to a computer, but with the help of NLP process it's possible for the computer to read, decipher, understand, and make sense of the human languages in a manner that is valuable.
NLP Techniques include:
* Named Entity Recognition
* Sentiment Analysis
* Text Summarization
* Aspect Mining
* Topic Modeling

In machine learning and natural language processing, a topic model is a statistical model used for discovering the abstract "topics" that occur in a collection of documents or in a corpus. A topic is a collection of dominant keywords that express the general meaning of the text.

NLP could be used to extract topics from reviews, social media feeds, comments, articles, emails as well as user feedbacks. Understanding what customers are talking about in a particular product is very vital to companies especially e-commerce industry. However, since these online reviews are quite often overwhelming in terms of numbers and information, an intelligent system, capable of finding key insights (topics) from these reviews, will be of great help for both customers and companies to get a feedback on their products like what is wrong in their product and what is good in their product. The goal of my project is to help customers make a decision when buying a product from amazon.in and help these product companies to understand what their customers are saying and make some improvements on their products.


One of the most effective ways of doing topic modeling is by using Gensim LDA model and we will be using it in this Project.

## About this Project

In this project I have web scrapped reviews of a random product from amazon.in. My purpose here is to apply text wrangling and text cleaning of the reviews then applying sentiment classification to them to see the percantage of positive, negative and neutral reviews.
Then I have used Topic Modeling to look for keywords about the product features in positive and negative reviews. For topic modeling I have used Latent Dirichlet Allocation model with hyperparamerter tuning of optimium number of topics based on the coherence value of the models.

Also, I am working on a web appliction to allow consumers to copy paste the link of a product on amazon.in and get the following results and visualization:
* Percentage of Positve & Negative reviews
* Top words based on frequency in the reviews
* Top Positive Reviews
* Top Negative Reviews
* Topic Model on Positive and Negative Reviews
* Wordcloud of Positive and Negative Reviews

# Tools And Technologies
1) NLTK libraries - Is used for text wrangling and preprocessing of the reviews. Tokenization, Lemmatization and Stopword removal.
2) Matplotlib and Plotly - For visualization and creating interactive plots.
3) Sklearn Countvectorizer - To create Term-Document Matrix
4) Gensim - Creating a LDA Model and hyperparameter tuning
5) pyLDAvis - Is used for LDA model visualization by approximating the features on a 2D plane
6) Vader Sentiment - I have used vader sentiment model for classifying reviews
7) Requests - For sending request and storing the response
8) Beautiful Soup -  For parsing html response

# Files in this Repository

* Amazon Product Scraping.ipynb	- Contains the scraping code
* Amazon_Reviews.csv	- Scraped Reviews for the random products
* LDA Model for Negative Reviews.zip	- Saved LDA model for Negative Reviews
* LDA Model for Positive Reviews.zip	- Saved LDA model for Positive Reviews
* LDA Model.zip	- LDA model on the whole review data
* Product Review Analysis.ipynb	- File containg Text Cleaning, Sentiment Classification, Topic Models and Interactive Plots
* Time series plot for number of reviews on each date.html	- Interactive time series plot for number of reviews on each date
* Top Negative Words in each topic.html	- LDA model Visualization for Negative Reviews
* Top Positive Words in each topic.html	- LDA model Visualization for Positive Reviews
* Top Words in each topic.html	- LDA Model Visualizatio for the whole review data
* Word cloud for Negative sentiment.png	
* Word cloud for Positive sentiment.png	
* cleaned_data.pkl	- Final cleaned data file
* sentiment_percentage_plot.html- Interactive sentiment Percentage Plot
* word_counts.png - Word count distribution plot

You can find the [Analysis File with Interactive Plots](https://nbviewer.jupyter.org/github/Shaan224/Topic-Modelling-on-Amazon-Product-Reviews/blob/master/Product%20Review%20Analysis.ipynb#)

# Scope of Improvement
This project is an effort to make an end to end project on NLP techniques starting from : **Data Collection -> Data Cleaning -> Data Storage and Access -> Exploratory Data Analysis -> Machine Learning -> Interpreting the Model -> Deployment and Implementation** 
I am new to this field and I am still learning about it. While using Vader Sentiment model for sentiment analysis there were some misclassification errors as some negative reviews with rating 1 or 2 were classified as positive reviews and some positive reviews with rating 4 or 5 were misclassified as negative reviews. Maybe we can solve this issue by adjusting the threshhold value for the model.
Any feedbacks or suggestions are welcome.
Thank You for viewing this Project :smile:
