# Sentiment Classification using LSTM

## Introduction
In this project, we build a recurrent neural network based sentiment classifier for movie reviews using LSTM (Long short term memory) units. We use the IMDB dataset which contains 50000 movie reviews.

## Methodology
Before starting with the learning process, the reviews had to be preprocessed and had to be converted into a set of word vectors/embeddings. After analysing the text corpus, it could be seen that there were some HTML tags, punctautions, extra spaces etc. That had to be removed.

Once the preprocessing was compelted, the words in the corpus had to be tokenised. There were nearly a 100,000 unique words in the entire dataset. Following that each word was mapped to its respective embeddings (we used the 100d Glove vectors in this project). The maximum length of the reviews was clipped at 100 words.

The dataset was then split into train and test sets at a 90-10 ratio. Following that, multiple NN architectures were tried for the task. To set a baseline, a simple neural network without LSTMs were tried first. Following that different configurations of LSTM layers along with other layers were tried.

## Results
Out of the models we tried, the network that gave the best performance and its accuracy score on the test  and train sets are given below.

![LSTM Network](https://github.com/muhammedsalihk/Sentiment-Classification-using-LSTM/blob/master/Images/download.png)

| Set | Accuracy Score |
| ------------- | ------------- |
| Test  | 0.8610  |
| Train  | 0.9019  |
| Validation  | 0.8640  |
