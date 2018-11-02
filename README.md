# Latent Semantic Analysis


The latent in Latent Semantic Analysis (LSA) means latent topics. 
Basically, LSA finds low-dimension representation of documents and words.
The dot product of row vectors is the document similarity, while the dot product of column vectors is the word similarity.
To reduce the dimensionality of X, apply truncated SVD. 
In this case, U ∈ ℝ^(m ⨉ t) emerges as our document-topic matrix, and V ∈ ℝ^(n ⨉ t) becomes our term-topic matrix. In both U and V, the columns correspond to one of our t topics. In U, rows represent document vectors expressed in terms of topics; in V, rows represent term vectors expressed in terms of topics.


Using:

            TfidfVectorizer
            TruncatedSVD

# LatentDirichletAllocation-Genism

LDA stands for Latent Dirichlet Allocation. LDA is a Bayesian version of pLSA. In particular, it uses dirichlet priors for the document-topic and word-topic distributions, lending itself to better generalization.
From a dirichlet distribution Dir(α), we draw a random sample representing the topic distribution, or topic mixture, of a particular document. This topic distribution is θ. From θ, we select a particular topic Z based on the distribution.
Next, from another dirichlet distribution Dir(𝛽), we select a random sample representing the word distribution of the topic Z. This word distribution is φ. From φ, we choose the word w.



Refer: https://medium.com/nanonets/topic-modeling-with-lsa-psla-lda-and-lda2vec-555ff65b0b05


This is implementation of LDA using Genism package. It retrieves topics from Newspaper JSON Data.

            Topics Found :

            1) Political-Wars 
            2) Computer 
            3) Countries 
            4) Aerospace 
            5) Crime and Law  
            6) Sports 
            7) Religion 

            Evaluation Used :

            1) Perplexity
            2) Coherence Score

(Tutorial Referred) Refer: https://www.machinelearningplus.com/nlp/topic-modeling-gensim-python/
