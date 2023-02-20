# TEXT_SUMMARIZATION_NLP
LANGUAGE USED: PYTHON 
LIBRARIES USED: 
         1.numpy
         2.pandas
         3.nltk(natural language tool kit)
         4.re(regular expression)
steps involved (overview):
     1.First, the text to be summarized is split into individual sentences using the sent_tokenize() function from the nltk library. The resulting list of sentences is          cleaned and preprocessed to remove any unwanted characters, convert all characters to lowercase, and remove any stopwords using Pandas, Numpy, and nltk.
     2.Next, the preprocessed sentences are converted into sentence vectors using pre-trained word embeddings such as GloVe.
     3.A similarity matrix is then constructed using the cosine similarity between pairs of sentence vectors.
     4.The similarity matrix is used to construct a graph representation of the text, where each sentence is a node and the cosine similarity between pairs of sentences        is the weight of the edge between them.
     5.The PageRank algorithm is applied to the graph to compute a score for each sentence that reflects its importance in the overall text.
     6.Finally, the most important sentences are selected based on their PageRank scores and used to generate a summary of the original text.
