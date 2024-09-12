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
    - Stop words are common words that are often removed from text processing tasks in Natural Language Processing (NLP) because they don't add much meaning and can make data less manageable. (from nltk.corpus import stopwords)

5. **Part of Speech(POS)**
    - Parts of Speech Categories:

      - Noun (NN): Refers to people, places, or things. (e.g., "dog", "city")
      - Verb (VB): Describes actions or states. (e.g., "run", "is")
      - Adjective (JJ): Describes attributes of nouns. (e.g., "happy", "blue")
      - Adverb (RB): Modifies verbs, adjectives, or other adverbs. (e.g., "quickly", "very")
      - Pronoun (PRP): Replaces nouns. (e.g., "he", "they")
      - Preposition (IN): Shows the relationship between a noun (or pronoun) and another word. (e.g., "on", "at")
      - Conjunction (CC): Connects words, phrases, or clauses. (e.g., "and", "but")
      - Interjection (UH): Expresses emotion. (e.g., "wow", "oops")

6. **Name Entry Recognition**
    - NER aims to locate and classify words or phrases in a text that represent entities into specific categories, such as:

       - Person: Names of people (e.g., "Barack Obama", "Albert Einstein")
       - Organization: Company names or institutions (e.g., "Google", "United Nations")
       - Location: Geographical locations (e.g., "Paris", "Mount Everest")
       - Date and Time: Specific dates and times (e.g., "January 1, 2020", "10:00 AM")
       - Monetary Values: Financial figures (e.g., "$1,000", "50 euros")
       - Percentages: (e.g., "20%", "15% increase")
       - Products: Names of products (e.g., "iPhone", "Tesla Model 3")
   
## **Machine Learning**:
1. One HOT Encoding
