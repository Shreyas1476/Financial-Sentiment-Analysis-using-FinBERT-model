# Financial-Sentiment-Analysis-using-FinBERT

Sentiment analysis, the process of determining the emotional tone behind a series of words, is a crucial component of natural language processing (NLP) with applications ranging from customer feedback interpretation to social media monitoring. In the financial sector, sentiment analysis helps in interpreting the language of market reports, financial news, and earnings calls, which in turn influences investment strategies and market predictions.
Traditional sentiment analysis tools, typically trained on general-purpose datasets like movie reviews or social media posts, lack the sophistication required for accurate financial sentiment analysis. They struggle with the intricacies of financial language, leading to suboptimal performance in identifying the sentiment in financial contexts. To address these challenges, domain-specific models are essential.

FinBERT, a specialized BERT model fine-tuned for financial sentiment analysis, addresses the unique language patterns and jargon prevalent in financial texts. By leveraging BERT’s foundational architecture and enhancing it with domain-specific data, FinBERT improves the accuracy of sentiment prediction in financial contexts.It is trained on the following three financial communication corpus. The total corpora size is 4.9B tokens.
+ Corporate Reports 10-K & 10-Q: 2.5B tokens
+ Earnings Call Transcripts: 1.3B tokens
+ Analyst Reports: 1.1B tokens

# Dataset Description :-

All datasets were downloaded from Kaggle :- 

1.Sentiment Analysis for Financial News dataset :-
This dataset (FinancialPhraseBank) contains the sentiments for financial news headlines from the perspective of a retail investor.The dataset contains two columns, "Sentiment" and "News Headline". The sentiment can be negative, neutral or positive.It contains a total of 4846 rows.Dataset link is https://www.kaggle.com/datasets/ankurzing/sentiment-analysis-for-financial-news/data

2.Financial Sentiment Analysis dataset :-
The dataset is intended for advancing financial sentiment analysis research. It's two datasets (FiQA, Financial PhraseBank) combined into one easy-to-use CSV file. It contains 5844 rows with 2 columns,”Sentence” and “Sentiment”. It provides financial sentences with sentiment labels.Dataset link is https://www.kaggle.com/datasets/sbhatti/financial-sentiment-analysis/data

# Methodology :-


