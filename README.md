# Financial-Sentiment-Analysis-using-FinBERT

Sentiment analysis, the process of determining the emotional tone behind a series of words, is a crucial component of natural language processing (NLP) with applications ranging from customer feedback interpretation to social media monitoring. In the financial sector, sentiment analysis helps in interpreting the language of market reports, financial news, and earnings calls, which in turn influences investment strategies and market predictions.

FinBERT, a specialized BERT model fine-tuned for financial sentiment analysis, addresses the unique language patterns and jargon prevalent in financial texts. By leveraging BERT’s foundational architecture and enhancing it with domain-specific data, FinBERT improves the accuracy of sentiment prediction in financial contexts.It is trained on the following three financial communication corpus. The total corpora size is 4.9B tokens.
+ Corporate Reports 10-K & 10-Q: 2.5B tokens
+ Earnings Call Transcripts: 1.3B tokens
+ Analyst Reports: 1.1B tokens

Here we have used two versions of the FinBERT model available in HuggingFace:-
+ ProsusAI FinBERT Model (https://huggingface.co/ProsusAI/finbert)
+ HKUST(yiyanghkust) FinBERT Model (https://huggingface.co/yiyanghkust/finbert-tone)

# Dataset Description :-

All datasets were downloaded from Kaggle :- 

1.Sentiment Analysis for Financial News dataset :-
This dataset (FinancialPhraseBank) contains the sentiments for financial news headlines from the perspective of a retail investor.The dataset contains two columns, "Sentiment" and "News Headline". The sentiment can be negative, neutral or positive.It contains a total of 4846 rows.Dataset link is https://www.kaggle.com/datasets/ankurzing/sentiment-analysis-for-financial-news/data

2.Financial Sentiment Analysis dataset :-
The dataset is intended for advancing financial sentiment analysis research. It's two datasets (FiQA, Financial PhraseBank) combined into one easy-to-use CSV file. It contains 5844 rows with 2 columns,”Sentence” and “Sentiment”. It provides financial sentences with sentiment labels.Dataset link is https://www.kaggle.com/datasets/sbhatti/financial-sentiment-analysis/data

# Methodology :-

Each of the sentences in both the datasets were directly subjected to the HuggingFace sentiment analysis pipeline.The pipelines are a great and easy way to use models for inference. These pipelines are objects that abstract most of the complex code from the library, offering a simple API dedicated to several tasks, including Named Entity Recognition, Masked Language Modeling, Sentiment Analysis, Feature Extraction and Question Answering.The pipeline simplifies the process of passing text through the tokenizer and model to generate sentiment predictions.

The accuracy of the predictions was computed using the accuracy_score function, and the confusion matrix was generated to assess the model's classification performance.

The model which gave higher accuracy on either of the datasets was chosen to be fine-tuned[12] for further enhancing its performance.It was generally observed that ProsusAI FinBERT Model gave better results than the HKUST(yiyanghkust) FinBERT Model. 

