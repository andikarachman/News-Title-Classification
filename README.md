# News Title Classification
In this notebook, we will classify news into categories based on their headline. Our goal is to identify whether a headline is belong to one of four classes: 
- Entertainment
- Business
- Technology
- Medical

To achieve that, we will use a recurrent neural network (RNN). Using an RNN rather than a strictly feedforward network is more accurate since we can include information about the *sequence* of words. We will use multiple bidirectional GRU/LSTM layers in the network. The bidirectional LSTM/GRU keeps the contextual information in both directions which is pretty useful in text classification task. We also use attention model to build our model architecture. 

In the past conventional methods like TFIDF/CountVectorizer etc., we used to find features from text by doing a keyword extraction. Some word are more helpful in determining the category of a text than others. But in this method we sort of lost the sequential structure of text. With LSTM and deep learning methods while we are able to take case of the sequence structure we lose the ability to give higher weightage to more important words. 

Additionally, attention mechanism is introduced to extract such words that are important to the meaning of the sentence and aggregate the representation of those informative words to form a sentence vector.
