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
