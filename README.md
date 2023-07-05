#Evaluating Feature Extraction Techniques for Optimal Latent Dirichlet Allocation Topic Modeling on the Scorius Dataset.


##Description
This GitHub repository has been created to provide support for a thesis project in Applied Data Science, authored by Emily van Veen.
The objective of this research is to identify the ideal feature extraction method for LDA topic modeling, specifically tailored to the Scorius dataset, to extract highly meaningful information. The research question following this investigation is: "Which feature extraction method produces the most effective results when applying Latent Dirichlet Allocation topic modeling to the Scorius dataset?"
Before conducting the topic modeling analysis, the data is cleaned. The preprocessing steps include removal of non-Dutch languages, tokenization, lemmatization, lowering the text data, removal of punctuations, special characters, numbers, emojis, removal of stopwords with an extended list, removal of words smaller than 3 characters, removal of missing values, and removal of excessive whitespaces. After preprocessing the data, the four final models were constructed, incorporating different variations of word combinations. These models included:
1. unigrams with all word combinations, 
2. unigrams with nouns only
3. bigrams with all word combinations
4. bigrams with nouns only. 
The optimal parameters for each model were calculated and are based on the relevant literature. To evaluate the models, two approaches were employed: the coherence score, which measures the semantic consistency of the topics, and the human interpretation of the model's output.
The model bigrams with all word combinations outperforms the other models on the two evaluation methods. 

##Files
The code in this project is written in the version Python 3.10.12
- Preprocessing file: This file contains the code for data preprocessing, including steps such as language removal, tokenization, lemmatization, lowercasing, removal of punctuation, special characters, numbers, and emojis, removal of stopwords, removal of words smaller than 3 characters, removal of missing values, and removal of excessive whitespaces. 
- Unigrams with all word combinations: This file contains the code for constructing the topic model using unigrams with all possible word combinations as the feature extraction method.
- Unigrams with nouns only: This file contains the code for constructing the topic model using unigrams with only nouns as the feature extraction method.
- Bigrams with all word combinations: This file contains the code for constructing the topic model using bigrams with all possible word combinations as the feature extraction method.
- Bigrams with nouns only: This file contains the code for constructing the topic model using bigrams with only nouns as the feature extraction method.
Each file includes data exploration to gain insights into the dataset. Furthermore, the parameter tuning is performed within each model file to optimize the model's performance.

##Usage
The research focused on analyzing the open-ended questions in the dataset, which consisted of two columns: one column for the questions and another for the corresponding answers.
Before running any of the model files, it is necessary to run the preprocessing file in order to clean the data and prepare it for topic modeling. The files contain comments that provide explanations and descriptions of the processes and actions taking place.

