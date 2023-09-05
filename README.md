![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)



# Sentiment Analysis of Customer Reviews

In today's hyperconnected digital landscape, data is more than just numbers and words; it's a window into the hearts and minds of your customers. Sentiment analysis aka Emotion AI, decodes the emotional opinions of consumers so that you can refine your marketing, optimize product offerings or promotions, and identify emerging trends

This is of special importance in CPG companies to stay competitive and as the voice of your customer changes.

## Demo 

![](https://github.com/aleivaar94/Customer-Review-Sentiment-Analysis-Streamlit/blob/master/assets/demo-sentiment.gif)


## Go To App [👆🏼](https://eminence-sentiment.streamlit.app/)


## Requirements

```
matplotlib==3.5.2
nltk==3.6.5
numpy==1.24.2
pandas==1.3.4
scipy==1.7.1
seaborn==0.11.2
streamlit==1.11.0
torch==1.12.0
transformers==4.20.1

```

## Methodology

### Data Collection

Data obtained from [Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews).

Dataset consists of ~500,000  reviews of fine foods from Amazon. The data span a period of more than 10 years, up to October 2012. Reviews include product and user information, ratings, and a plain text review.

<sup>J. McAuley and J. Leskovec. <ins>From amateurs to connoisseurs: modeling the evolution of user expertise through online reviews.</ins> WWW, 2013.</sup>


### Data Analysis

1. Data Preprocessing: Clean and prepare the text data, including removing noise and irrelevant information.

1.1 Tokenization

1.2 Stop Word Removal

1.3 Stemming or Lemmatization

2. Compare Sentiment Analysis Models: VADER (Valence Aware Dictionaru and Sentiment Reasoner) vs Huggingface 🤗 RoBERTAv(Robustly Optimized BERT Pretraining Approach) model


2. Sentiment Analysis: Apply sentiment analysis usings [Huggingface 🤗](https://huggingface.co/docs/transformers/model_doc/roberta#transformers.TFRobertaForQuestionAnswering) RoBERTA model.

![](https://github.com/aleivaar94/Customer-Review-Sentiment-Analysis-Streamlit/blob/master/assets/vader-CI.png)

![](https://github.com/aleivaar94/Customer-Review-Sentiment-Analysis-Streamlit/blob/master/assets/Roberta-CI.png)


<sup>Top: Vader accuracy. Bottom: RoBERTA accuracy.  RoBERTA model is more accurate</sup>

You can find the Streamlit app code in `Customer_Review_Sentiment.py`


Follow the jupyter notebook to see the methodology in detail:

```
sentiment.ipynb
```

