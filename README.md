# **Experiment No. 16**
## **Title : NLP Techniques on Text Data in Python**

## **Introduction**
Natural Language Processing (NLP) is a branch of Artificial Intelligence that enables computers to understand, interpret, and process human language. Text data is unstructured and contains punctuation, stopwords, and variations in word forms, making it difficult to use directly.
This experiment demonstrates fundamental NLP preprocessing techniques using the NLTK library. These techniques convert raw text into a structured format suitable for tasks like sentiment analysis, text classification, and spam detection.


## **Requirements**
Install required library: nltk
Download necessary resources such as tokenizer, stopwords, wordnet, and POS tagger


## **Theory and Concepts**


###### 1. Tokenization
Tokenization is the process of splitting text into smaller units such as words or sentences.
- Word Tokenization: Splits text into individual words
- Sentence Tokenization: Splits paragraph into sentences
Syntax:
- word_tokenize(text)
- sent_tokenize(text)

 
###### 2. Stop Word Removal
Stop words are commonly used words that carry little meaning and can be removed to reduce noise.
- Helps in improving efficiency of models
- Reduces unnecessary data
 Syntax:
- [w for w in tokens if w.lower() not in stopwords]


###### 3. Stemming
Stemming reduces words to their root form using rule-based techniques.
- Faster process
- May produce non-dictionary words
Syntax:
- PorterStemmer().stem(word)


###### 4. Lemmatization

Lemmatization converts words into their base form using vocabulary and context.
- Produces valid dictionary words
- More accurate but slower
Syntax:
- WordNetLemmatizer().lemmatize(word)

Stemming vs Lemmatization
Stemming
- Rule-based suffix removal
- Faster
- Less accurate
Lemmatization
- Uses dictionary lookup
- Slower
- More accurate

  
###### 5. Part-of-Speech (POS) Tagging
POS tagging assigns grammatical labels to each word.
- Identifies nouns, verbs, adjectives, etc.
- Helps in understanding sentence structure
Syntax:
- pos_tag(tokens)


###### 6. Word Frequency Count
Counts how many times each word appears in text.
- Helps identify important words
- Useful in text analysis and feature extraction
Syntax:
- FreqDist(tokens)


###### NLP Preprocessing Pipeline
- Raw Text
- Tokenization
- Lowercasing
- Stop Word Removal
- Punctuation Removal
- Stemming or Lemmatization
- POS Tagging
- Clean Structured Text
###### Libraries Used
- nltk → Core NLP operations
- nltk.tokenize → Tokenization
- nltk.corpus → Stopwords
- nltk.stem → Stemming and Lemmatization
- nltk.probability → Frequency analysis

- 
## **Conclusion**
This experiment demonstrates key NLP preprocessing techniques used to convert raw text into structured data.
- Tokenization forms the base of NLP processing
- Stop word removal reduces noise
- Stemming and lemmatization simplify words
- POS tagging helps understand grammar
- Frequency analysis highlights important words
These techniques together prepare text data for machine learning and real-world NLP applications.
