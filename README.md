# NLP Practice

This repository focuses on Natural Language Processing (NLP) techniques in both Machine Learning (ML) and Deep Learning (DL). Below is an overview of key concepts and methods:

### **ML-based NLP Techniques**
1. **Text Preprocessing**:
   - **Tokenization**: Splitting text into smaller units (tokens) such as words or sentences.
   - **Stemming**: Reducing words to their root forms (e.g., "eating" to "eat").
   - **Lemmatization**: Similar to stemming but more accurate, converting words to their base form.
   - **Bag of Words (BoW)**: Representing text as a collection of words without considering order.
   - **TF/IDF**: Term Frequency-Inverse Document Frequency, a method for weighting terms.
   - **N-grams**: A continuous sequence of `n` words (e.g., Unigram = 1 word, Bigram = 2 words).
   - **Word2Vec & AvgWord2Vec**: Techniques to represent words as vectors.

### **DL-based NLP Techniques**
1. **RNN, LSTM RNN, GRU RNN**: Recurrent Neural Networks used for sequential data like text.
2. **Text Preprocessing (Word Embeddings)**: Using embeddings like Word2Vec for representing text.
3. **Transformer Models**: Attention-based models for processing entire sentences at once.
4. **BERT (Bidirectional Encoder Representations from Transformers)**: A powerful transformer-based model that understands context.

## **Text Preprocessing**

1. **Tokenization**
   - Separates words from sentences or paragraphs, aiding further processing.
   - Common types:
     - **Sent Tokenization**: Splits text into sentences.(from nltk.tokenize import sent_token)
     - **Word Tokenization**: Splits text into words (recommended for most use cases).(from nltk.tokenize import word_token)
     - **WordPunct Tokenization**: Splits words and punctuations separately.(from nltk.tokenize import wordpunct_token)
     - **Tree Bank Word Tokenization**:The Treebank tokenizer uses regular expressions to tokenize text as in Penn Treebank.(from nltk.tokenize import TreebankWordTokenizer)

2. **Stemming**
   - Converts words to their root form. Example: "eating" becomes "eat".
   - Common Types:
     - **Porter Stemming**: A widely used algorithm for stemming in English.(from nltk.stem import PorterStemmer)
     - **Regular expression Stemmer**: Uses regular expressions to determine word stems.(from nltk.stem import RegExpStemmer)
     - **Snowball Stemmer**: An updated and more efficient version of Porter Stemmer.(from nltk.stem import SnowballStemmer)

3. **Lemmetization**
    - it is like stemming but advance version of it as it will give us a exact word that will be validated word
    - Common types:
      - **WordNetLemmetizer**: Provides 3 lemmatizer modes: _morphy(), morphy() and lemmatize(). lemmatize() is a permissive wrapper around _morphy(). It returns the shortest lemma found in WordNet, or the input string unchanged if nothing is found.(from nltk.stem import WordNetLemmatizer)
      
4. **Stop Words**
    - 
   
