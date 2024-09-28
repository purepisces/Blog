## Question 1

**What is NLP?**

NLP stands for Natural Language Processing. The subfield of Artificial intelligence and computational linguistics deals with the interaction between computers and human languages. It involves developing algorithms, models, and techniques to enable machines to understand, interpret, and generate natural languages in the same way as a human does.

NLP encompasses a wide range of tasks, including language translation, sentiment analysis, text categorization, information extraction, speech recognition, and natural language understanding. NLP allows computers to extract meaning, develop insights, and communicate with humans in a more natural and intelligent manner by processing and analyzing textual input.


## Question 2

**What are the main challenges in NLP?**

The complexity and variety of human language create numerous difficult problems for the study of Natural Language Processing (NLP). The primary challenges in NLP are as follows:

- Semantics and Meaning: It is a difficult undertaking to accurately capture the meaning of words, phrases, and sentences. The semantics of the language, including word sense disambiguation, metaphorical language, idioms, and other linguistic phenomena, must be accurately represented and understood by NLP models.
- Ambiguity: Language is ambiguous by nature, with words and phrases sometimes having several meanings depending on context. Accurately resolving this ambiguity is a major difficulty for NLP systems.
- Contextual Understanding: Context is frequently used to interpret language. For NLP models to accurately interpret and produce meaningful replies, the context must be understood and used. Contextual difficulties include, for instance, comprehending referential statements and resolving pronouns to their antecedents.
- Language Diversity: NLP must deal with the world’s wide variety of languages and dialects, each with its own distinctive linguistic traits, lexicon, and grammar. The lack of resources and knowledge of low-resource languages complicates matters.
- Data Limitations and Bias: The availability of high-quality labelled data for training NLP models can be limited, especially for specific areas or languages. Furthermore, biases in training data might impair model performance and fairness, necessitating careful consideration and mitigation.
- Real-world Understanding: NLP models often fail to understand real-world knowledge and common sense, which humans are born with. Capturing and implementing this knowledge into NLP systems is a continuous problem.


## 🌟 Question 3

**What are the different tasks in NLP?**

Natural Language Processing (NLP) includes a wide range of tasks involving understanding, processing, and creation of human language. Some of the most important tasks in NLP are as follows:

-   [Text Classification](https://www.geeksforgeeks.org/classification-of-text-documents-using-the-approach-of-naive-bayes)
-   [Named Entity Recognition (NER)](https://www.geeksforgeeks.org/python-named-entity-recognition-ner-using-spacy)
-   [Part-of-Speech Tagging (POS)](https://www.geeksforgeeks.org/nlp-part-of-speech-default-tagging)
-   [Sentiment Analysis](https://www.geeksforgeeks.org/what-is-sentiment-analysis)
-   [Language Modeling](https://www.geeksforgeeks.org/videos/what-is-language-modelling-in-nlp)
-   [Machine Translation](https://www.geeksforgeeks.org/machine-translation-of-languages-in-artificial-intelligence)
-   [Chatbots](https://www.geeksforgeeks.org/battle-of-ai-chatbots-which-chatbot-will-rule-the-present-and-future)
-   [Text Summarization](https://www.geeksforgeeks.org/python-extractive-text-summarization-using-gensim)
-   [Information Extraction](https://www.geeksforgeeks.org/difference-between-information-retrieval-and-information-extraction)
-   [Text Generation](https://www.geeksforgeeks.org/text-generation-using-recurrent-long-short-term-memory-network)
-   [Speech Recognition](https://www.geeksforgeeks.org/text-generation-using-recurrent-long-short-term-memory-network)

## Question 4

**What do you mean by Corpus in NLP?**

In NLP, a [corpus](https://www.geeksforgeeks.org/nlp-wordlist-corpus) is a huge collection of texts or documents. It is a structured dataset that acts as a sample of a specific language, domain, or issue. A corpus can include a variety of texts, including books, essays, web pages, and social media posts. Corpora are frequently developed and curated for specific research or NLP objectives. They serve as a foundation for developing language models, undertaking linguistic analysis, and gaining insights into language usage and patterns.


## Question 5

**What do you mean by text augmentation in NLP and what are the different text augmentation techniques in NLP?**

[Text augmentation](https://www.geeksforgeeks.org/text-augmentation-techniques-in-nlp) in NLP refers to the process that generates new or modified textual data from existing data in order to increase the diversity and quantity of training samples. Text augmentation techniques apply numerous alterations to the original text while keeping the underlying meaning.

Different text augmentation techniques in NLP include:

1.  ****Synonym Replacement:**** Replacing words in the text with their synonyms to introduce variation while maintaining semantic similarity.
2.  ****Random Insertion/Deletion:**** Randomly inserting or deleting words in the text to simulate noisy or incomplete data and enhance model robustness.
3.  ****Word Swapping:**** Exchanging the positions of words within a sentence to generate alternative sentence structures.
4.  ****Back translation:**** Translating the text into another language and then translating it back to the original language to introduce diverse phrasing and sentence constructions.
5.  ****Random Masking:**** Masking or replacing random words in the text with a special token, akin to the approach used in masked language models like BERT.
6.  ****Character-level Augmentation:**** Modifying individual characters in the text, such as adding noise, misspellings, or character substitutions, to simulate real-world variations.
7.  ****Text Paraphrasing:**** Rewriting sentences or phrases using different words and sentence structures while preserving the original meaning.
8.  ****Rule-based Generation:**** Applying linguistic rules to generate new data instances, such as using grammatical templates or syntactic transformations.

### Example 
**1. Synonym Replacement**

In this technique, words in a sentence are replaced with their synonyms to introduce variation while keeping the meaning intact.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Synonym Replacement**:  
"The fast brown fox leaps over the lazy dog."

**2. Random Insertion**

This method involves randomly inserting words that are semantically relevant into the sentence.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Random Insertion**:  
"The quick brown fox jumps swiftly over the lazy dog."

**3. Random Deletion**

Random words are deleted from the sentence to simulate incomplete or noisy data.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Random Deletion**:  
"Quick brown fox jumps over dog."

**4. Word Swapping**

In word swapping, words are swapped within a sentence to create different sentence structures without changing the overall meaning.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Word Swapping**:  
"Over the lazy dog, the quick brown fox jumps."

**5. Back Translation**

A sentence is translated into another language and then translated back into the original language, resulting in slightly different phrasing.

**Original Sentence (English)**:  
"The quick brown fox jumps over the lazy dog."

**Translated to French**:  
"Le renard brun rapide saute par-dessus le chien paresseux."

**Back to English**:  
"The fast brown fox leaps over the lazy dog."

 **6. Random Masking**

In this technique, random words in a sentence are replaced by a special token, similar to the technique used in models like BERT.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Random Masking**:  
"The quick [MASK] fox jumps over the [MASK] dog."

**7. Character-level Augmentation**

At the character level, random modifications are made to individual characters to simulate typos or real-world text variations.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Character-level Augmentation**:  
"The quick bronw fox jmups over the lazy dog."

**8. Text Paraphrasing**

Paraphrasing changes the sentence structure and wording while keeping the same meaning.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Paraphrased Text**:  
"A fast, brown fox leaps across the lazy dog."

**9. Rule-based Generation**

This involves applying specific linguistic rules to create new text. For example, you can change verb tenses or rearrange sentence structures.

**Original Sentence**:  
"The quick brown fox jumps over the lazy dog."

**Rule-based Generation (change tense)**:  
"The quick brown fox jumped over the lazy dog."

## Question 6

**What are some common pre-processing techniques used in NLP?**

[Natural Language Processing (NLP)](https://www.geeksforgeeks.org/natural-language-processing-nlp-pipeline) preprocessing refers to the set of processes and techniques used to prepare raw text input for analysis, modelling, or any other NLP tasks. The purpose of preprocessing is to clean and change text data so that it may be processed or analyzed later.

Preprocessing in NLP typically involves a series of steps, which may include:

-   [Tokenization](https://www.geeksforgeeks.org/tokenize-text-using-nltk-python)
-   [Stop Word Removal](https://www.geeksforgeeks.org/removing-stop-words-nltk-python)
-   [Text Normalization](https://www.geeksforgeeks.org/normalizing-textual-data-with-python)
    -   Lowercasing
    -   Lemmatization
    -   Stemming
    -   Date and Time Normalization
-   [Removal of Special Characters and Punctuation](https://www.geeksforgeeks.org/removing-punctuations-given-string)
-   [Removing HTML Tags or Markup](https://www.geeksforgeeks.org/program-to-remove-html-tags-from-a-given-string)
-   [Spell Correction](https://www.geeksforgeeks.org/correcting-words-using-nltk-in-python)
-   [Sentence Segmentation](https://www.geeksforgeeks.org/python-perform-sentence-segmentation-using-spacy)


1. **Tokenization**

Tokenization is the process of breaking down a sentence or document into individual words or phrases, known as tokens. This helps in analyzing the text at a more granular level.

**Example**:  
Original Text: "The quick brown fox jumps over the lazy dog."  
After Tokenization: `["The", "quick", "brown", "fox", "jumps", "over", "the", "lazy", "dog"]`

2. **Stop Word Removal**

Stop words are common words (such as "the", "is", "in", "at") that do not carry significant meaning and are removed to focus on the important words.

**Example**:  
Original Text: "The quick brown fox jumps over the lazy dog."  
After Stop Word Removal: `["quick", "brown", "fox", "jumps", "lazy", "dog"]`

3. **Text Normalization**

Text normalization involves converting text into a standard format. This process includes several steps:

-   **Lowercasing**: Converting all text to lowercase to ensure uniformity.
    
    **Example**:  
    Original Text: "The QUICK Brown Fox."  
    After Lowercasing: `"the quick brown fox"`
    
-   **Lemmatization**: Reducing words to their base form (lemma) while maintaining the context.
    
    **Example**:  
    Original Word: "running"  
    After Lemmatization: `"run"`
    Original Word: "better"
    After Lemmatization: `"good"`
    
-   **Stemming**: Reducing words to their root form, often leading to truncation.
    
    **Example**:  
    Original Word: "running"  
    After Stemming: `"run"`
    Original Word: "studies"
    After Stemming: `"studi"`
 In the second example, stemming produced `"studi"`, which is not a valid word.
    
-   **Date and Time Normalization**: Converting dates and times into a consistent format.
    
    **Example**:  
    Original Text: "I was born on 20th June, 1995."  
    After Date Normalization: `"I was born on [DATE]."`
    

4. **Removal of Special Characters and Punctuation**

Special characters and punctuation marks are usually removed as they do not carry significant meaning in most NLP tasks.

**Example**:  
Original Text: "Hello! How are you doing today?"  
After Removal of Special Characters: `"Hello How are you doing today"`

5. **Removing HTML Tags or Markup**

When working with web-scraped data, removing HTML tags is essential to extract clean text for analysis.

**Example**:  
Original Text: "<p>This is a paragraph.</p>"  
After Removing HTML Tags: `"This is a paragraph."`

6. **Spell Correction**

This involves correcting spelling mistakes in the text.

**Example**:  
Original Text: "The quik brown fox jmps over the lazi dog."  
After Spell Correction: `"The quick brown fox jumps over the lazy dog."`

7. **Sentence Segmentation**

Sentence segmentation is the process of dividing text into individual sentences.

**Example**:  
Original Text: "The quick brown fox jumps. It is very agile."  
After Sentence Segmentation:  
`["The quick brown fox jumps.", "It is very agile."]`

## Question 7
**What is text normalization in NLP?**

Text normalization, also known as text standardization, is the process of transforming text data into a standardized or normalized form It involves applying a variety of techniques to ensure consistency, reduce variations, and simplify the representation of textual information.

The goal of text normalization is to make text more uniform and easier to process in Natural Language Processing (NLP) tasks. Some common techniques used in text normalization include:

-   ****Lowercasing****: Converting all text to lowercase to treat words with the same characters as identical and avoid duplication.
-   ****Lemmatization****: Converting words to their base or dictionary form, known as lemmas. For example, converting “running” to “run” or “better” to “good.”
-   ****Stemming****: Reducing words to their root form by removing suffixes or prefixes. For example, converting “playing” to “play” or “cats” to “cat.”
-   ****Abbreviation Expansion****: Expanding abbreviations or acronyms to their full forms. For example, converting “NLP” to “Natural Language Processing.”
-   ****Numerical Normalization****: Converting numerical digits to their written form or normalizing numerical representations. For example, converting “100” to “one hundred” or normalizing dates.
-   ****Date and Time Normalization****: Standardizing date and time formats to a consistent representation.


## Reference
- https://www.geeksforgeeks.org/nlp-interview-questions/

