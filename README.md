## Natural Language Processing

**NLP Data Cleaning Techniques:**

_Basic:_

1. Removing punctuation like !,#
2. Convert to lower case
3. Removing stopwords as does not have much value. Stopwords are common words like (a,the,is,to)
4. Removing nonsocial word like new line
5. Tokenization of the text (Can be character based, sentence word)Tokenization means dividing text into smaller parts.
6. Lemmatization and Stemming but it's completely depends on use case. Stemming is like stem or root of the word
   Stemming merely removes common suffixes from the end of word tokens, lemmatization ensures the output word is an existing normalized form of the word (for example, lemma) that can be found in the dictionary

_Advance:_

1. Normalization - like b4,ttyl - to English word before. There are libraries that we can use to do this normalization
2. Correcting typos - Not easy to implement.

**Feature Extraction:**

1. Corpus: A corpus is a collection of texts that represent a language
2. Bag of Words(BOW): Unique count of words in corpus
3. Few Problems in Feature extraction during vectorization:
   - Will have 0 for words that does not exist in other documents
   - Frequency of a text can be more that can be resolve by normalization(Occurence/total_no_of_words)
   - Common words can have more cout than other and can supress the actual meaning of text so to solve this use TF-IDF.
4. TF-IDF(Term Frequency-Inverse Document Frequency): It quantify the importance of a term in a document with respect to its frequency in the document and its rarity across multiple documents. **TF-IDF(t,d,D)=TF(t,d)×IDF(t,D)**

**Word Embeddings:** Word embeddings are a way to represent words as vectors of numbers, where words with similar meanings are represented by similar vectors.
The basic vector embedding is **One Hot Encoding** where 1 stands for the position where the word exists and 0 everywhere else.
_Ex: ["My ,"Name" ,"is", "Vipul". here vector embedding for "Vipul" will be [0,0,0,1]_

**Note:** Problem with this approach is that for large number of documents it will have more 0's so it will be diffcult to process and get the meaning out of it)

Different Type of Word Embeddings:

- Frequency-based Embedding (Count Vector,TF-IDF,Co-Occurrence)
- Prediction-based Embedding (CBOW (Continuous Bag of words),Skip – Gram)
