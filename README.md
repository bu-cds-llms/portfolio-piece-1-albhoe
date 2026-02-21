A Comparison of Prediction Models in Natural Language Processing

This lab compares the 'Bag of Words', 'TF-IDF' methods of representing text by comparing their ability to distinguish between positive and negative movie reviews. This was done using Naive Bayesian classification based on the similarity to reviews in the training dataset according to these metrics.
Additionally, N-Grams were used to create a word prediction system, which uses Naive Bayes prediction and a stochastic chain of tokens to predict the next most probable word. This was performed in sequence to mimic the 'style' of the sentences in a training dataset. 
These models were optimized by fine tuning hyperparameters (max_features,drop_words) iteratively. 

Key Results: The highest accuracy I was able to achieve was eighty eight point two percent, using Term Frequency - Inverse Document Frequency analysis on the eight thousand most common words after dropping the ninety most common. I also noticed a significant increase in runtime with vocabularies larger than ten thousand words; although, accuracy showed little to no change past this point. Although I expected Term Frequency - Inverse Document Frequency analysis to perform more accurately overall, I did not expect that this analysis would be improved by ignoring common words, as the Inverse Document Frequency analysis already takes common but unimportant words into account. I am curious which analysis technique would excel at this task. I suspect that random forest would be suited for classifying based on individual words by directly analyzing which words create the most prominent split.

<img width="1300" height="791" alt="image" src="https://github.com/user-attachments/assets/77d9f03e-fb9b-40c1-9293-624941acd0fa" />

The notebook downloads the necessary dataset through a url or contains hardcoded inputs. It can simply be run in a python3 environment.

The packages used are: urllib.request, tarfile, os, numpy, pandas, collections, typing, re, sklearn, random, and collections.
