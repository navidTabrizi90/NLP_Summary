# Summarization 

## Table of Contents

-   [Overview](#overview)
-   [Pipeline](#pipeline)
-   [Dependencies](#dependencies)
-   [Result](#result)

## Overview

 Text Summarization Using Natural Language

### Pipeline

1.  **Text Data**: A user submits a section of text for summarization

2.  **Tokenization**: The original text is segmented into sentences using NLTK's sent_tokenize function. NLTK's word_tokenize function breaks down the text into individual words

3. **Stopword Removal**:Common English stopwords like "the" and "is" along with non-alphanumeric words are eliminated using NLTK's stopwords list to emphasize significant words

4. **Word Frequency Calculation**: The occurrence of each remaining word is computed using NLTK's FreqDist function

5. **Sentence Evaluation**: Each sentence is evaluated based on the frequency of its words. The score of a sentence is the average word frequency within it, indicating its importance

6. **Sentence Selection**: Sentences are ranked according to their scores. The top-ranked sentences are picked to create the summary. The number of sentences chosen is based on the context window limit, considering the average sentence length

7. **Summary Generation**: The chosen sentences are combined to produce the summary. If the resulting summary exceeds the context window limit, it is shortened to fit within the boundary. Result: The final condensed text is presented to the user.
## Dependencies

-   Python 
-   nltk
-   nltk.probability
-   nltk.corpus


## Result

The final summarized text is output to the user# NLP_Summary
