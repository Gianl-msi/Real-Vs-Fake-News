# Real-Vs-Fake-News
<img src="https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/images/word%20cloud.JPG" width="500" height="250"/>


### Table of Contents
- [Abstract](#Abstract)
- [Datasets](#Datasets)
- [Docs](#Docs)
- [Notebooks](#Notebooks)
- [Conclusions and Future Directions](#Conclusions-and-Future-Directions)

---

## Abstract
The unchecked spreading of fake news is an alarming phenomenon on every social media platform and information outlet. Since online content can have a decisive effect on users’ political, social and business decisions and opinions, the identification and elimination of false information has become a critical prerogative for many online companies.

Natural language processing (NLP) encompasses linguistics, computer science, information engineering, and artificial intelligence. The main application of NLP is to train algorithms to analyze texts and extrapolated actionable insights based on text’s word composition and frequency. Another way of examining a document is analyzing the document’s intrinsic complexity. Text complexity is measured by several linguistic indexes such as Flesch Kincaid and Coleman Liau indexes.

Herein, I tested several machine learning models that leverage NLP techniques, linguistic indexes or both, to predict the news’ truthiness. The best model I built was able to discriminate real from fake news with a balanced accuracy of 0.9779 and AUC score of 0.9992.

## Datasets
Real and fake news datasets can be found here(https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset
).

## [Docs](https://github.com/Gianl-msi/Real-Vs-Fake-News/tree/master/Docs)
- [Exploratory Data Analysis](https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/Docs/Fake%20News%20-%20EDA%208-30.pdf)
- [Final Report](https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/Docs/Fake%20news%20-%20Final%20report%209-6.pdf)
- [Presentation](https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/Docs/Fake%20news%20presentation.pdf)


## [Notebooks](https://github.com/Gianl-msi/Real-Vs-Fake-News/tree/master/Notebooks)
- [Data Wrangling](https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/Notebooks/Real%20and%20Fake%20News%20-%20DW_8-30.ipynb)
- [Exploratory Data Analysis](https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/Notebooks/Real%20and%20Fake%20News%20-%20EDA%20-%208-30.ipynb)
- [Modeling](https://github.com/Gianl-msi/Real-Vs-Fake-News/blob/master/Notebooks/Real%20and%20Fake%20News%20-%20Preprocessing%20%26%20Modeling%208-30.ipynb)

## Conclusions and Future Directions
The unchecked spreading of fake information has become a real problem for social media platforms and online information outlets, and it has prompted data science and machine learning communities to develop precise tools for identification and successive removal of untrue information. Herein, I created and tested several models for the accurate discrimination of real news from fake news. These modeIs leveraged NLP techniques as well as linguistic complexity and indexes of title and text of the news. 

One important limitation of this study is that real and fake news were collected from two different sources, suggesting that difference in these sources may have made prediction easier than it should be. I dove into the data to attempt to find any clear markers that differentiated these two sources, but even after these steps were taken my overall AUC score remained over .99 which seems unlikely to be true in reality. For future studies, ideally, we could either collect real and fake news articles (as labelled by a third party) from a similar distribution of sources, or we could pull articles from a few sources and use crowdsourcing to label them as real or fake. 

There are additional steps that could be taken to improve the predictive power of the model which I couldn’t take given the limitations of computational complexity and runtime. First, I could lower min_df to include rare words. Another feature that could be added is the amount of punctuation in the text of the document. Fake news’ text tends to have an excess of exclamation marks, asterisks and other punctuation marks. The text could also be analyzed for spelling and grammar errors. Finally, a more sophisticated vectorizer such as word2vec could be implemented to maintain and analyze words’ semantic in text and title of the news. 

In conclusion I developed a high performing machine learning model for the discrimination of real from fake news. While my model may have some limitations, several courses of action exist to improve its robustness, reliability and predictive power.






