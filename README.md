# LatentDirichletAllocation-Genism

LDA stands for Latent Dirichlet Allocation. LDA is a Bayesian version of pLSA. In particular, it uses dirichlet priors for the document-topic and word-topic distributions, lending itself to better generalization.
From a dirichlet distribution Dir(α), we draw a random sample representing the topic distribution, or topic mixture, of a particular document. This topic distribution is θ. From θ, we select a particular topic Z based on the distribution.
Next, from another dirichlet distribution Dir(𝛽), we select a random sample representing the word distribution of the topic Z. This word distribution is φ. From φ, we choose the word w.



Refer: https://medium.com/nanonets/topic-modeling-with-lsa-psla-lda-and-lda2vec-555ff65b0b05


This is implementation of LDA using Genism package. It retrieves topics from Newspaper JSON Data.
1) Remove emails and newline characters
2) Tokenize words and Clean-up text
3) Remove Stopwords, Make Bigrams and Lemmatize
4) Create the Dictionary and Corpus needed for Topic Modeling
5) Compute Model Perplexity and Coherence Score
6) Visualize the topics-keywords
7) Building LDA Mallet Model
8) Optimal number of topics for LDA
9) Dominant topic in each sentence

Refer: https://www.machinelearningplus.com/nlp/topic-modeling-gensim-python/
