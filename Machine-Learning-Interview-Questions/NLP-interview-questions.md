need to look at fine tune: https://nbviewer.org/github/DrRuin/Lightweight-Fine-Tuning/blob/main/Lightweight-Fine-Tuning.ipynb

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



## Question 8

**What is tokenization in NLP?**

[Tokenization](https://www.geeksforgeeks.org/tokenization-using-spacy-library) is the process of breaking down text or string into smaller units called tokens. These tokens can be words, characters, or subwords depending on the specific applications. It is the fundamental step in many natural language processing tasks such as sentiment analysis, machine translation, and text generation. etc.

Some of the most common ways of tokenization are as follows:

-   ****Sentence tokenization:**** In Sentence tokenizations, the text is broken down into individual sentences. This is one of the fundamental steps of tokenization.
-   ****Word tokenization:**** In word tokenization, the text is simply broken down into words. This is one of the most common types of tokenization. It is typically done by splitting the text into spaces or punctuation marks.
-   ****Subword tokenization:**** In subword tokenization, the text is broken down into subwords, which are the smaller part of words. Sometimes words are formed with more than one word, for example, Subword i.e Sub+ word, Here sub, and words have different meanings. When these two words are joined together, they form the new word “subword”, which means “a smaller unit of a word”. This is often done for tasks that require an understanding of the morphology of the text, such as stemming or lemmatization.
-   ****Char-label tokenization:**** In Char-label tokenization, the text is broken down into individual characters. This is often used for tasks that require a more granular understanding of the text such as text generation, machine translations, etc.


## Question 9

**What is NLTK and How it’s helpful in NLP?**

[NLTK](https://www.geeksforgeeks.org/python-nltk-tokenize-regexp) stands for Natural Language Processing Toolkit. It is a suite of libraries and programs written in Python Language for symbolic and statistical natural language processing. It offers tokenization, stemming, lemmatization, POS tagging, Named Entity Recognization, parsing, semantic reasoning, and classification.

NLTK is a popular NLP library for Python. It is easy to use and has a wide range of features. It is also open-source, which means that it is free to use and modify.

### Key Features of NLTK:

1.  **Tokenization**: NLTK allows you to break down text into smaller units, such as sentences or words.
2.  **Stemming**: It provides stemmers like the Porter Stemmer to reduce words to their root form.
3.  **Lemmatization**: NLTK offers tools to reduce words to their dictionary form, accounting for context.
4.  **POS Tagging**: NLTK can assign part-of-speech (POS) tags to words in a sentence, such as noun, verb, adjective, etc.
5.  **Named Entity Recognition (NER)**: NLTK can recognize proper nouns and categorize them as organizations, people, or locations.
6.  **Parsing**: It allows for syntactic parsing of sentences to understand sentence structure.
7.  **Classification**: NLTK provides tools to classify text into categories (e.g., spam or non-spam).
8.  **Text Corpora**: NLTK includes many well-known corpora (collections of text data) such as the Brown Corpus, Gutenberg Corpus, and WordNet for word relations.

### Example of NLTK in Action:

#### 1. **Tokenization Example**:

```python
import nltk
nltk.download('punkt')  # Download necessary data
from nltk.tokenize import word_tokenize

text = "Natural Language Processing with NLTK is easy."
tokens = word_tokenize(text)
print(tokens)
```

**Output**:
```css
['Natural', 'Language', 'Processing', 'with', 'NLTK', 'is', 'easy', '.']
```
#### 2.**POS Tagging Example**:
```python
nltk.download('averaged_perceptron_tagger')
from nltk import pos_tag

tokens = word_tokenize("NLTK helps in processing text.")
tagged = pos_tag(tokens)
print(tagged)
```
**Output**:
```css
[('NLTK', 'NNP'), ('helps', 'VBZ'), ('in', 'IN'), ('processing', 'VBG'), ('text', 'NN'), ('.', '.')]
```
Here, NLTK has tagged each word with its corresponding part of speech (e.g., NNP for proper noun, VBZ for verb).

#### 3. **Named Entity Recognition Example**:
```python
nltk.download('maxent_ne_chunker')
nltk.download('words')
from nltk import ne_chunk

sentence = "Apple is looking at buying a startup in New York."
tokens = word_tokenize(sentence)
tagged = pos_tag(tokens)
entities = ne_chunk(tagged)
print(entities)
```
**Output**:
```css
(S
  (ORGANIZATION Apple/NNP)
  is/VBZ
  looking/VBG
  at/IN
  buying/VBG
  a/DT
  startup/NN
  in/IN
  (GPE New/NNP York/NNP)
  ./.)
```
Here, NLTK identifies "Apple" as an **organization** and "New York" as a **geopolitical entity (GPE)**.

## Questoin 10

**What is stemming in NLP, and how is it different from lemmatization?**

Stemming and lemmatization are two commonly used word normalization techniques in NLP, which aim to reduce the words to their base or root word. Both have similar goals but have different approaches.

In [stemming](https://www.geeksforgeeks.org/python-stemming-words-with-nltk), the word suffixes are removed using the heuristic or pattern-based rules regardless of the context of the parts of speech. The resulting stems may not always be actual dictionary words. Stemming algorithms are generally simpler and faster compared to lemmatization, making them suitable for certain applications with time or resource constraints.

In [lemmatization](https://www.geeksforgeeks.org/python-lemmatization-with-nltk), The root form of the word known as lemma, is determined by considering the word’s context and parts of speech. It uses linguistic knowledge and databases (e.g., wordnet) to transform words into their root form. In this case, the output lemma is a valid word as per the dictionary. For example, lemmatizing “running” and “runner” would result in “run.” Lemmatization provides better interpretability and can be more accurate for tasks that require meaningful word representations.


## Question 11

**How does part-of-speech tagging work in NLP?**

[Part-of-speech tagging](https://www.geeksforgeeks.org/part-speech-tagging-stop-words-using-nltk-python) is the process of assigning a part-of-speech tag to each word in a sentence. The POS tags represent the syntactic information about the words and their roles within the sentence.

There are three main approaches for POS tagging:

-   ****Rule-based POS tagging:**** It uses a set of handcrafted rules to determine the part of speech based on morphological, syntactic, and contextual patterns for each word in a sentence. For example, words ending with ‘-ing’ are likely to be a verb.
-   ****Statistical POS tagging:**** The statistical model like Hidden Markov Model (HMMs) or Conditional Random Fields (CRFs) are trained on a large corpus of already tagged text. The model learns the probability of word sequences with their corresponding POS tags, and it can be further used for assigning each word to a most likely POS tag based on the context in which the word appears.
-   ****Neural network POS tagging:**** The neural network-based model like RNN, LSTM, Bi-directional RNN, and transformer have given promising results in POS tagging by learning the patterns and representations of words and their context.


Part-of-speech (POS) tagging is the process of labeling each word in a sentence with its corresponding part of speech, such as noun, verb, adjective, etc. This helps machines understand the syntactic role of each word in context. There are three main approaches to POS tagging: rule-based, statistical, and neural network-based methods.

### Example Sentence:

_"The quick brown fox jumps over the lazy dog."_

#### 1. **Rule-based POS Tagging:**

Rule-based POS tagging uses hand-crafted linguistic rules to assign tags based on word patterns and context. For example:

-   "The" is identified as a determiner because it commonly precedes nouns.
-   Words ending with "-ing" or "-ed" are often tagged as verbs.
-   "Quick" is tagged as an adjective because it modifies "fox."

In the sentence:

-   **The** (determiner)
-   **quick** (adjective)
-   **brown** (adjective)
-   **fox** (noun)
-   **jumps** (verb)
-   **over** (preposition)
-   **the** (determiner)
-   **lazy** (adjective)
-   **dog** (noun)

The rules here identify parts of speech based on word structure and position in the sentence.

#### 2. **Statistical POS Tagging:**

Statistical methods, such as Hidden Markov Models (HMMs) or Conditional Random Fields (CRFs), use a probabilistic model that has been trained on large datasets. The model looks at the likelihood of a word being a specific POS tag based on its context. For example, the word "fox" is more likely to be a noun if it follows an adjective like "quick."

For the sentence:

-   The statistical model might predict "jumps" is a verb because the likelihood of seeing a verb after the noun "fox" is high, based on training data.

#### 3. **Neural Network POS Tagging:**

Neural networks, especially models like Recurrent Neural Networks (RNNs), Long Short-Term Memory (LSTM), or Transformers, have achieved state-of-the-art results in POS tagging. These models can capture long-term dependencies in a sentence, understanding both the word itself and its context within the entire sentence.

For example, a Bi-directional LSTM might:

-   Look at the word "jumps" and analyze not just the preceding words ("fox") but also the following words ("over") to make a more accurate prediction that "jumps" is a verb.

Neural models can also handle ambiguous words better. For example, "fox" could be either a noun or a verb, but based on context, neural models predict it as a noun in this case.

### Summary of Example:

-   **Rule-based:** Relies on fixed linguistic patterns (e.g., suffixes or word order).
-   **Statistical:** Predicts based on the likelihood of word sequences from previously tagged data.
-   **Neural networks:** Understands the deeper context of a word's role in the sentence using advanced machine learning techniques.


## Question 12

**What is named entity recognition in NLP?**

[Named Entity Recognization (NER)](https://www.geeksforgeeks.org/named-entity-recognition) is a task in natural language processing that is used to identify and classify the named entity in text. Named entity refers to real-world objects or concepts, such as persons, organizations, locations, dates, etc. NER is one of the challenging tasks in NLP because there are many different types of named entities, and they can be referred to in many different ways. The goal of NER is to extract and classify these named entities in order to offer structured data about the entities referenced in a given text.

The approach followed for Named Entity Recognization (NER) is the same as the POS tagging. The data used while training in NER is tagged with persons, organizations, locations, and dates.

### Example:

For the sentence:  
_"Barack Obama was born in Hawaii on August 4, 1961, and became the President of the United States."_

NER would identify:

-   **"Barack Obama"** as a **Person**,
-   **"Hawaii"** as a **Location**,
-   **"August 4, 1961"** as a **Date**, and
-   **"President of the United States"** as an **Organization** or title.

### How NER Works:

NER uses similar techniques as Part-of-Speech (POS) tagging, but instead of tagging grammatical roles, it focuses on identifying named entities. There are three main approaches for NER:

1.  **Rule-based NER**: Uses manually crafted rules such as regular expressions or linguistic patterns to identify entities. For example, names may start with a capital letter, or dates might follow certain formats (e.g., "DD-MM-YYYY"). This approach lacks flexibility for unseen cases but works well for highly structured data.
    
2.  **Statistical NER**: Similar to POS tagging, statistical methods like Hidden Markov Models (HMMs) or Conditional Random Fields (CRFs) are trained on large datasets where entities are already labeled. The model learns the probability of a word belonging to a certain entity type based on its context and can predict entity tags in unseen text. For instance, it might learn that "Barack" followed by "Obama" is likely a person’s name.
    
3.  **Neural Network-based NER**: More recent methods use deep learning techniques like Recurrent Neural Networks (RNNs), Long Short-Term Memory (LSTM), or Transformer models like BERT. These models can capture complex patterns and long-range dependencies in the text. For example, a neural network model could use the broader context of "President" to correctly identify "United States" as a location or entity even if it's used in a less obvious form.


## Question 13
**What is parsing in NLP?**

In NLP, [parsing](https://www.geeksforgeeks.org/difference-between-top-down-parsing-and-bottom-up-parsing) is defined as the process of determining the underlying structure of a sentence by breaking it down into constituent parts and determining the syntactic relationships between them according to formal grammar rules. The purpose of parsing is to understand the syntactic structure of a sentence, which allows for deeper learning of its meaning and encourages different downstream NLP tasks such as semantic analysis, information extraction, question answering, and machine translation. it is also known as syntax analysis or syntactic parsing.

The formal grammar rules used in parsing are typically based on Chomsky’s hierarchy. The simplest grammar in the Chomsky hierarchy is regular grammar, which can be used to describe the syntax of simple sentences. More complex grammar, such as context-free grammar and context-sensitive grammar, can be used to describe the syntax of more complex sentences.


### 14. What are the different types of parsing in NLP?

In natural language processing (NLP), there are several types of parsing algorithms used to analyze the grammatical structure of sentences. Here are some of the main types of parsing algorithms:

-   [****Constituency Parsing****](https://www.geeksforgeeks.org/constituency-parsing-and-dependency-parsing): Constituency parsing in NLP tries to figure out a sentence’s hierarchical structure by breaking it into constituents based on a particular grammar. It generates valid constituent structures using context-free grammar. The parse tree that results represents the structure of the sentence, with the root node representing the complete sentence and internal nodes representing phrases. Constituency parsing techniques like as CKY, Earley, and chart parsing are often used for parsing. This approach is appropriate for tasks that need a thorough comprehension of sentence structure, such as semantic analysis and machine translation. When a complete understanding of sentence structure is required, constituency parsing, a classic parsing approach, is applied.
-   [****Dependency Parsing****](https://www.geeksforgeeks.org/constituency-parsing-and-dependency-parsing)****:**** In NLP, dependency parsing identifies grammatical relationships between words in a sentence. It represents the sentence as a directed graph, with dependencies shown as labelled arcs. The graph emphasises subject-verb, noun-modifier, and object-preposition relationships. The head of a dependence governs the syntactic properties of another word. Dependency parsing, as opposed to constituency parsing, is helpful for languages with flexible word order. It allows for the explicit illustration of word-to-word relationships, resulting in a clear representation of grammatical structure.
-   [****Top-down parsing:****](https://www.geeksforgeeks.org/difference-between-top-down-parsing-and-bottom-up-parsing) Top-down parsing starts at the root of the parse tree and iteratively breaks down the sentence into smaller and smaller parts until it reaches the leaves. This is a more natural technique for parsing sentences. However, because it requires a more complicated language, it may be more difficult to implement.
-   [****Bottom-up parsing:****](https://www.geeksforgeeks.org/difference-between-top-down-parsing-and-bottom-up-parsing) Bottom-up parsing starts with the leaves of the parse tree and recursively builds up the tree from smaller and smaller constituents until it reaches the root. Although this method of parsing requires simpler grammar, it is frequently simpler to implement, even when it is less understandable.


### Example:

Consider the sentence:  
_"The quick brown fox jumps over the lazy dog."_

-   **Parsing** this sentence involves identifying the syntactic components (constituents), such as the **subject** ("The quick brown fox"), **verb** ("jumps"), and **prepositional phrase** ("over the lazy dog").
-   The parse tree would show the hierarchical structure where "The quick brown fox" is the **noun phrase**, "jumps" is the **verb**, and "over the lazy dog" is a **prepositional phrase** that modifies the verb.

### Types of Parsing in NLP

#### 1. **Constituency Parsing**:

Constituency parsing focuses on dividing a sentence into **constituents** (phrases or sub-phrases) based on a formal grammar, often using context-free grammar (CFG). The goal is to build a **parse tree** that represents the sentence structure with nodes for each phrase and subphrase.

-   **Example:** For the sentence _"The cat sits on the mat,"_ constituency parsing breaks it down into:
    -   "The cat" (Noun Phrase)
    -   "sits" (Verb Phrase)
    -   "on the mat" (Prepositional Phrase)

The parse tree would start from the sentence at the root, with branches representing the **Noun Phrase (NP)** and **Verb Phrase (VP)**.

#### 2. **Dependency Parsing**:

Dependency parsing analyzes the **dependencies** between words in a sentence. It represents the sentence as a **directed graph**, where the nodes are words and the edges represent grammatical relationships, such as **subject-verb** or **verb-object**.

-   **Example:** For the sentence _"The cat chased the mouse,"_ dependency parsing would show:
    -   "cat" as the **subject** of the verb "chased"
    -   "mouse" as the **object** of the verb "chased"

The dependency graph shows how each word depends on others (e.g., the verb "chased" governs both "cat" and "mouse").

#### 3. **Top-down Parsing**:

In top-down parsing, the parsing process starts at the **root of the parse tree** (representing the whole sentence) and progressively breaks the sentence into smaller parts (phrases or words) according to grammar rules, moving down toward the leaves (individual words).

-   **Example:** For the sentence _"She ate an apple,"_ the top-down parser would start by dividing it into a **Noun Phrase (She)** and **Verb Phrase (ate an apple)**. It would then further divide the verb phrase into a verb ("ate") and an object ("an apple").

#### 4. **Bottom-up Parsing**:

In bottom-up parsing, the parser starts at the **leaves** (the individual words of the sentence) and attempts to combine them into larger constituents until the entire sentence is covered and the root of the tree is formed.

-   **Example:** For the sentence _"They watch movies,"_ the bottom-up parser would start with the individual words:
    -   "They" (Pronoun)
    -   "watch" (Verb)
    -   "movies" (Noun)

It then gradually combines these into phrases (e.g., "watch movies" as a verb phrase), eventually reaching the full parse tree that represents the sentence.

### Comparing Top-down and Bottom-up Parsing:

-   **Top-down parsing** breaks the sentence from the root into smaller components, which makes it more intuitive but can struggle with ambiguous or complex grammars.
-   **Bottom-up parsing** builds the tree from individual words, making it easier to implement but potentially less intuitive when trying to understand the entire sentence structure.


## Question 15

**What do you mean by vector space in NLP?**

In natural language processing (NLP), A [vector space](https://www.geeksforgeeks.org/web-information-retrieval-vector-space-model) is a mathematical vector where words or documents are represented by numerical vectors form. The word or document’s specific features or attributes are represented by one of the dimensions of the vector. Vector space models are used to convert text into numerical representations that machine learning algorithms can understand.

Vector spaces are generated using techniques such as word embeddings, bag-of-words, and term frequency-inverse document frequency (TF-IDF). These methods allow for the conversion of textual data into dense or sparse vectors in a high-dimensional space. Each dimension of the vector may indicate a different feature, such as the presence or absence of a word, word frequency, semantic meaning, or contextual information.


### Example 1: Bag-of-Words Model

Let's take the following three simple sentences:

1.  **"I love cats"**
2.  **"I love dogs"**
3.  **"Cats are great"**

In the **bag-of-words (BoW)** model, we create a vector space where each unique word in the corpus (all sentences combined) is represented as a dimension. For these sentences, the unique words are: `["I", "love", "cats", "dogs", "are", "great"]`. This gives us a 6-dimensional vector space.

Now, we can represent each sentence as a vector:

-   Sentence 1: "I love cats" → `[1, 1, 1, 0, 0, 0]` (1 for the words "I", "love", and "cats" being present, and 0 for others).
-   Sentence 2: "I love dogs" → `[1, 1, 0, 1, 0, 0]` (1 for the words "I", "love", and "dogs", 0 for others).
-   Sentence 3: "Cats are great" → `[0, 0, 1, 0, 1, 1]` (1 for the words "cats", "are", and "great", 0 for others).

In this vector space, each sentence is represented as a 6-dimensional vector, where the dimensions correspond to the words in the corpus.

### Example 2: Word Embeddings

In **word embeddings** (e.g., Word2Vec or GloVe), the words are represented as vectors in a continuous, high-dimensional vector space. These vectors capture semantic meaning, and similar words will have vectors that are close to each other in this space.

For example, the words **"king"**, **"queen"**, **"man"**, and **"woman"** might be represented in a vector space where:

-   The vector for **"king"** could be `[0.6, 0.2, 0.8]`.
-   The vector for **"queen"** could be `[0.6, 0.2, 0.7]`.
-   The vector for **"man"** might be `[0.4, 0.1, 0.9]`.
-   The vector for **"woman"** might be `[0.4, 0.1, 0.8]`.

The closeness of these vectors (in terms of cosine similarity) tells us that **"king"** and **"queen"** are semantically related, as are **"man"** and **"woman"**.

### Example 3: TF-IDF

The **TF-IDF (Term Frequency-Inverse Document Frequency)** method represents words in a vector space by assigning higher weights to words that are frequent in a specific document but less frequent across the whole corpus.

For instance, in a document about "machine learning," common words like "machine" and "learning" will have high term frequencies in the document but low frequencies in the entire corpus (because they are specific to this topic), thus having higher TF-IDF scores.

In the TF-IDF vector space, each document will be represented by a vector where each dimension corresponds to a word, and the value of the dimension is the **TF-IDF score** of that word in the document.

## Question 16
**What is the bag-of-words model?**

[Bag of Words](https://www.geeksforgeeks.org/bag-of-words-bow-model-in-nlp) is a classical text representation technique in NLP that describes the occurrence of words within a document or not. It just keeps track of word counts and ignores the grammatical details and the word order.

Each document is transformed as a numerical vector, where each dimension corresponds to a unique word in the vocabulary. The value in each dimension of the vector represents the frequency, occurrence, or other measure of importance of that word in the document.

Let's consider two simple text documents:  
Document 1: "I love apples."  
Document 2: "I love mangoes too."  
  
Step 1: Tokenization  
Document 1 tokens: ["I", "love", "apples"]  
Document 2 tokens: ["I", "love", "mangoes", "too"]  
  
Step 2: Vocabulary Creation by collecting all unique words across the documents  
Vocabulary: ["I", "love", "apples", "mangoes", "too"]  
The vocabulary has five unique words, so each document vector will have five dimensions.  
  
Step 3: Vectorization  
Create numerical vectors for each document based on the vocabulary.  
For Document 1:  
- The dimension corresponding to "I" has a value of 1.  
- The dimension corresponding to "love" has a value of 1.  
- The dimension corresponding to "apples" has a value of 1.  
- The dimensions corresponding to "mangoes" and "too" have values of 0 since they do not appear in Document 1.  
Document 1 vector: [1, 1, 1, 0, 0]  
  
For Document 2:  
- The dimension corresponding to "I" has a value of 1.  
- The dimension corresponding to "love" has a value of 1.  
- The dimension corresponding to "mangoes" has a value of 1.  
- The dimension corresponding to "apples" has a value of 0 since it does not appear in Document 2.  
- The dimension corresponding to "too" has a value of 1.  
Document 2 vector: [1, 1, 0, 1, 1]  

The value in each dimension represents the occurrence or frequency of the corresponding word in the document. The BoW representation allows us to compare and analyze the documents based on their word frequencies.

## Question 17

**Define the Bag of N-grams model in NLP.**

The [Bag of n-grams](https://www.geeksforgeeks.org/n-gram-language-modelling-with-nltk) model is a modification of the standard bag-of-words (BoW) model in NLP. Instead of taking individual words to be the fundamental units of representation, the Bag of n-grams model considers contiguous sequences of n words, known as n-grams, to be the fundamental units of representation.

The Bag of n-grams model divides the text into n-grams, which can represent consecutive words or characters depending on the value of n. These n-grams are subsequently considered as features or tokens, similar to individual words in the BoW model.

The steps for creating a bag-of-n-grams model are as follows:

-   The text is split or tokenized into individual words or characters.
-   The tokenized text is used to construct N-grams of size n (sequences of n consecutive words or characters). If n is set to 1 known as uni-gram i.e. same as a bag of words, 2 i.e. bi-grams, and 3 i.e. tri-gram.
-   A vocabulary is built by collecting all unique n-grams across the entire corpus.
-   Similarly to the BoW approach, each document is represented as a numerical vector. The vector’s dimensions correspond to the vocabulary’s unique n-grams, and the value in each dimension denotes the frequency or occurrence of that n-gram in the document.


### Explain
The **Bag of N-grams** model is an extension of the **Bag of Words (BoW)** model in Natural Language Processing (NLP), where instead of looking at individual words, it considers **contiguous sequences of 'n' words** (called **n-grams**) as the fundamental unit of representation. This allows the model to capture word **sequences** or **context**, which the standard BoW model ignores.

### Key Difference:

-   In the **Bag of Words (BoW)** model, each word is treated independently.
-   In the **Bag of N-grams** model, sequences of words (e.g., pairs or triples of consecutive words) are considered, helping capture some level of word order or phrase-level information.

### How the Bag of N-grams Model Works:

1.  **Tokenization**: The text is broken into individual tokens (words or characters).
2.  **N-grams Formation**: The tokenized text is grouped into **n-grams**, which are sequences of **n consecutive tokens** (words). The value of **n** determines the size of the n-gram:
    -   **Unigram (n = 1)**: Single words (same as Bag of Words).
    -   **Bigram (n = 2)**: Pairs of consecutive words.
    -   **Trigram (n = 3)**: Triples of consecutive words.
3.  **Vocabulary Creation**: A vocabulary of all unique n-grams is created across the entire corpus.
4.  **Vectorization**: Each document is represented as a vector where the dimensions correspond to the unique n-grams, and the values represent the frequency or occurrence of those n-grams in the document.

### Example:

Let’s consider two simple documents:

**Document 1**: "I love apples"  
**Document 2**: "I love mangoes too"

#### Step 1: Tokenization

Both documents are tokenized into individual words:

-   Document 1 tokens: ["I", "love", "apples"]
-   Document 2 tokens: ["I", "love", "mangoes", "too"]

#### Step 2: N-grams Formation

Let’s create **bigrams** (n = 2) for both documents:

-   **Document 1 Bigrams**:
    -   "I love"
    -   "love apples"
-   **Document 2 Bigrams**:
    -   "I love"
    -   "love mangoes"
    -   "mangoes too"

#### Step 3: Vocabulary Creation

The vocabulary is created by gathering all the unique bigrams from both documents:

-   **Vocabulary**: ["I love", "love apples", "love mangoes", "mangoes too"]

#### Step 4: Vectorization

Now, we create vectors for each document based on the frequency of these bigrams in each document.

-   **Document 1 Vector**:
    
    -   "I love" appears 1 time → 1
    -   "love apples" appears 1 time → 1
    -   "love mangoes" appears 0 times → 0
    -   "mangoes too" appears 0 times → 0  
        **Vector**: [1, 1, 0, 0]
-   **Document 2 Vector**:
    
    -   "I love" appears 1 time → 1
    -   "love apples" appears 0 times → 0
    -   "love mangoes" appears 1 time → 1
    -   "mangoes too" appears 1 time → 1  
        **Vector**: [1, 0, 1, 1]

### Why Use N-grams?

-   **Capturing Word Sequences**: Unlike BoW, which ignores word order, **N-grams** can capture word order and local context. For instance, "I love" vs. "love I" are treated as different bigrams, preserving some context.
-   **Short Phrases**: N-grams can capture commonly occurring phrases like "New York" or "machine learning," which might be missed by individual word representations.
-   **Balance Between Complexity and Context**: Unigrams lose context, and higher-order n-grams (like trigrams or 4-grams) can become computationally expensive. **Bigrams** or **trigrams** provide a balance between context and simplicity.

### Example Comparison (Unigram vs. Bigram):

For Document 1 ("I love apples"):

-   **Unigram (n=1) representation (Bag of Words)**:  
    Vocabulary: ["I", "love", "apples", "mangoes", "too"]  
    Document vector: [1, 1, 1, 0, 0] (word occurrences)
    
-   **Bigram (n=2) representation (Bag of N-grams)**:  
    Vocabulary: ["I love", "love apples", "love mangoes", "mangoes too"]  
    Document vector: [1, 1, 0, 0] (bigram occurrences)
    

In the bigram model, you capture that **"I love"** and **"love apples"** are consecutive, which gives more information about the structure of the sentence.

### Summary:

The **Bag of N-grams** model extends the BoW model by incorporating sequences of words (n-grams), allowing it to capture some word order and context, which can be crucial for tasks like text classification, machine translation, and sentiment analysis.

## Question 18

**What is the term frequency-inverse document frequency (TF-IDF)?**

[Term frequency-inverse document frequency (TF-IDF)](https://www.geeksforgeeks.org/understanding-tf-idf-term-frequency-inverse-document-frequency) is a classical text representation technique in NLP that uses a statistical measure to evaluate the importance of a word in a document relative to a corpus of documents. It is a combination of two terms: term frequency (TF) and inverse document frequency (IDF).

-   ****Term Frequency (TF):**** Term frequency measures how frequently a word appears in a document. it is the ratio of the number of occurrences of a term or word (t ) in a given document (d) to the total number of terms in a given document (d). A higher term frequency indicates that a word is more important within a specific document.
-   ****Inverse Document Frequency (IDF):**** Inverse document frequency measures the rarity or uniqueness of a term across the entire corpus. It is calculated by taking the logarithm of the ratio of the total number of documents in the corpus to the number of documents containing the term. it down the weight of the terms, which frequently occur in the corpus, and up the weight of rare terms.

The TF-IDF score is calculated by multiplying the term frequency (TF) and inverse document frequency (IDF) values for each term in a document. The resulting score indicates the term’s importance in the document and corpus. Terms that appear frequently in a document but are uncommon in the corpus will have high TF-IDF scores, suggesting their importance in that specific document.

## Question 19

**Explain the concept of cosine similarity and its importance in NLP.**

The similarity between two vectors in a multi-dimensional space is measured using the cosine similarity metric. To determine how similar or unlike the vectors are to one another, it calculates the cosine of the angle between them.

In natural language processing (NLP), [Cosine similarity](https://www.geeksforgeeks.org/cosine-similarity) is used to compare two vectors that represent text. The degree of similarity is calculated using the cosine of the angle between the document vectors. To compute the cosine similarity between two text document vectors, we often used the following procedures:

-   Text Representation: Convert text documents into numerical vectors using approaches like bag-of-words, TF-IDF (Term Frequency-Inverse Document Frequency), or word embeddings like Word2Vec or GloVe.
-   Vector Normalization: Normalize the document vectors to unit length. This normalization step ensures that the length or magnitude of the vectors does not affect the cosine similarity calculation.
-   Cosine Similarity Calculation: Take the dot product of the normalised vectors and divide it by the product of the magnitudes of the vectors to obtain the cosine similarity.

Mathematically, the cosine similarity between two document vectors, **a** and **b** , can be expressed as:

$$\text{Cosine Similarity}(\vec{a}, \vec{b}) = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}$$

Here,

-   $\vec{a} \cdot \vec{b}$ is the dot product of vectors a and b
-   |a| and |b| represent the Euclidean norms (magnitudes) of vectors a and b, respectively.

The resulting cosine similarity score ranges from -1 to 1, where 1 represents the highest similarity, 0 represents no similarity, and -1 represents the maximum dissimilarity between the documents.


### Example: Cosine Similarity in Action

Let's consider two small text documents:

-   **Document 1**: "I love apples."
-   **Document 2**: "I love mangoes."

#### Step 1: Text Representation (Bag of Words)

First, convert these documents into vectors using the **Bag of Words** method. The vocabulary based on these two documents is: ["I", "love", "apples", "mangoes"].

-   Document 1: **"I love apples"** → [1, 1, 1, 0]
-   Document 2: **"I love mangoes"** → [1, 1, 0, 1]

Here, each dimension represents a word in the vocabulary, and the value is the count of the word's occurrence in the document.

#### Step 2: Cosine Similarity Calculation

Now, we calculate the cosine similarity between the two vectors **[1, 1, 1, 0]** (Document 1) and **[1, 1, 0, 1]** (Document 2).

1.  **Dot Product**:

$$\vec{a} \cdot \vec{b} = (1 \times 1) + (1 \times 1) + (1 \times 0) + (0 \times 1) = 1 + 1 + 0 + 0 = 2$$


2.  **Magnitude of Vector a (Document 1)**:
$$|\vec{a}| = \sqrt{(1^2 + 1^2 + 1^2 + 0^2)} = \sqrt{3} \approx 1.732$$

3.  **Magnitude of Vector b (Document 2)**:
$$|\vec{b}| = \sqrt{(1^2 + 1^2 + 0^2 + 1^2)} = \sqrt{3} \approx 1.732$$

4.  **Cosine Similarity**:
$$\text{Cosine Similarity}(\vec{a}, \vec{b}) = \frac{2}{1.732 \times 1.732} = \frac{2}{3} \approx 0.6667$$

#### Result:

The cosine similarity between **Document 1** ("I love apples") and **Document 2** ("I love mangoes") is **0.6667**, which indicates a moderate level of similarity. This makes sense because both documents share two words ("I" and "love"), but differ in their fruit choice.

## Question 20

**What are the differences between rule-based, statistical-based and neural-based approaches in NLP?**

[Natural language processing (NLP)](https://www.geeksforgeeks.org/natural-language-processing-nlp-pipeline) uses three distinct approaches to tackle language understanding and processing tasks: rule-based, statistical-based, and neural-based.

1.  ****Rule-based Approach:**** Rule-based systems rely on predefined sets of linguistic rules and patterns to analyze and process language.
    -   Linguistic Rules are manually crafted rules by human experts to define patterns or grammar structures.
    -   The knowledge in rule-based systems is explicitly encoded in the rules, which may cover syntactic, semantic, or domain-specific information.
    -   Rule-based systems offer high interpretability as the rules are explicitly defined and understandable by human experts.
    -   These systems often require manual intervention and rule modifications to handle new language variations or domains.
2.  ****Statistical-based Approach:**** Statistical-based systems utilize statistical algorithms and models to learn patterns and structures from large datasets.
    -   By examining the data’s statistical patterns and relationships, these systems learn from training data.
    -   Statistical models are more versatile than rule-based systems because they can train on relevant data from various topics and languages.
3.  ****Neural-based Approach:**** Neural-based systems employ deep learning models, such as neural networks, to learn representations and patterns directly from raw text data.
    -   Neural networks learn hierarchical representations of the input text, which enable them to capture complex language features and semantics.
    -   Without explicit rule-making or feature engineering, these systems learn directly from data.
    -   By training on huge and diverse datasets, neural networks are very versatile and can perform a wide range of NLP tasks.
    -   In many NLP tasks, neural-based models have attained state-of-the-art performance, outperforming classic rule-based or statistical-based techniques.


#### Example of Rule-based Approach:

A rule-based system for identifying dates in text may use a regular expression like `DD-MM-YYYY` to extract dates. For instance, given the sentence **"My birthday is on 10-12-1995."**, the system will recognize **"10-12-1995"** as a date using predefined patterns.

#### Limitation:

If the date format changes to **"10th of December, 1995"**, the system may fail unless a new rule is added to handle this variation.

#### Example of Statistical-based Approach:

A **Hidden Markov Model (HMM)** used for Part-of-Speech (POS) tagging may learn that in a sentence like **"The cat sits"**, the word **"cat"** is likely to be a noun based on its context and probability distribution.

#### Limitation:

Statistical-based approaches may struggle when there is insufficient data or when encountering rare language patterns not seen in training data.

#### Example of Neural-based Approach::

A **Transformer-based model** like BERT can be used to solve multiple NLP tasks, such as **question answering**. If asked **"What is the capital of France?"**, the model will likely output **"Paris"** by learning semantic relationships and contextual clues from vast amounts of text data.

#### Limitation:

Neural models require large datasets and significant computational power for training. They can also be opaque, making it hard to interpret their decisions.


### Comparison with Examples:

| **Aspect**            | **Rule-based Approach**                | **Statistical-based Approach**        | **Neural-based Approach**             |
|-----------------------|----------------------------------------|---------------------------------------|---------------------------------------|
| **Method**            | Manually defined linguistic rules      | Learns from statistical patterns      | Learns representations with deep learning |
| **Data Requirement**  | Requires less data                     | Needs moderate amounts of data        | Requires large datasets               |
| **Interpretability**  | Highly interpretable                   | Moderate, probabilistic explanations  | Hard to interpret, "black-box" models |
| **Flexibility**       | Not adaptable to new domains/languages | Adaptable with enough data            | Highly adaptable but data-hungry      |
| **Example Task**      | Rule-based POS tagging (predefined rules) | POS tagging with HMM (probabilistic tagging) | POS tagging with BERT (contextual tagging) |

### Example:
Consider the task of **Part-of-Speech (POS) tagging** for the sentence: **"I am learning NLP."**

- **Rule-based approach**: Manually defined grammar rules identify **"I"** as a pronoun, **"am"** as a verb, **"learning"** as a verb, and **"NLP"** as a noun based on syntax rules.
  
- **Statistical-based approach**: A probabilistic model like an **HMM** assigns POS tags based on learned word patterns and their likelihood of occurring together.
  
- **Neural-based approach**: A model like **BERT** understands the context and automatically tags **"I"** as a pronoun, **"am"** as a verb, **"learning"** as a verb, and **"NLP"** as a noun based on deep contextual embeddings.

### Summary:
- **Rule-based systems** use predefined linguistic rules but struggle with new language patterns.
- **Statistical-based models** rely on probabilistic learning from data and handle more variation but require significant data.
- **Neural-based models** learn representations and patterns from raw text data, often achieving the best performance, but they require large datasets and computational power.


## Question 21

**What do you mean by Sequence in the Context of NLP?**

A Sequence primarily refers to the sequence of elements that are analyzed or processed together. In [NLP](https://www.geeksforgeeks.org/natural-language-processing-nlp-pipeline), a sequence may be a sequence of characters, a sequence of words or a sequence of sentences.

In general, sentences are often treated as sequences of words or tokens. Each word in the sentence is considered an element in the sequence. This sequential representation allows for the analysis and processing of sentences in a structured manner, where the order of words matters.

By considering sentences as sequences, NLP models can capture the contextual information and dependencies between words, enabling tasks such as part-of-speech tagging, named entity recognition, sentiment analysis, machine translation, and more.

## 🌟 Question 22

**What are the various types of machine learning algorithms used in NLP?**

There are various types of machine learning algorithms that are often employed in natural language processing (NLP) tasks. Some of them are as follows:

-   [Naive Bayes:](https://www.geeksforgeeks.org/naive-bayes-classifiers) Naive Bayes is a probabilistic technique that is extensively used in NLP for text classification tasks. It computes the likelihood of a document belonging to a specific class based on the presence of words or features in the document.
-   [Support Vector Machines (SVM)](https://www.geeksforgeeks.org/support-vector-machine-algorithm): SVM is a supervised learning method that can be used for text classification, sentiment analysis, and named entity recognition. Based on the given set of features, SVM finds a hyperplane that splits data points into various classes.
-   [Decision Trees:](https://www.geeksforgeeks.org/decision-tree) Decision trees are commonly used for tasks such as sentiment analysis, and information extraction. These algorithms build a tree-like model based on an order of decisions and feature conditions, which helps in making predictions or classifications.
-   [Random Forests:](https://www.geeksforgeeks.org/random-forest-classifier-using-scikit-learn) Random forests are a type of ensemble learning that combines multiple decision trees to improve accuracy and reduce overfitting. They can be applied to the tasks like text classification, named entity recognition, and sentiment analysis.
-   [Recurrent Neural Networks (RNN):](https://www.geeksforgeeks.org/introduction-to-recurrent-neural-network) RNNs are a type of neural network architecture that are often used in sequence-based NLP tasks like language modelling, machine translation, and sentiment analysis. RNNs can capture temporal dependencies and context within a word sequence.
-   [Long Short-Term Memory (LSTM)](https://www.geeksforgeeks.org/long-short-term-memory-lstm-rnn-in-tensorflow): LSTMs are a type of recurrent neural network that was developed to deal with the vanishing gradient problem of RNN. LSTMs are useful for capturing long-term dependencies in sequences, and they have been used in applications such as machine translation, named entity identification, and sentiment analysis.
-   [Transformer](https://www.geeksforgeeks.org/transformer-neural-network-in-deep-learning-overview): Transformers are a relatively recent architecture that has gained significant attention in NLP. By exploiting self-attention processes to capture contextual relationships in text, transformers such as the BERT (Bidirectional Encoder Representations from Transformers) model have achieved state-of-the-art performance in a wide range of NLP tasks.


### 1. **Naive Bayes**

**Naive Bayes** is a probabilistic algorithm often used for text classification tasks. It calculates the probability of a document belonging to a particular class based on the presence of words or features in the document. The algorithm assumes that the presence of each word in the document is independent of the others, which is called the **naive** assumption.

-   **Example**:
    
    -   **Task**: Spam classification in emails.
    -   Given an email with the words "free," "money," and "win," Naive Bayes can predict whether the email is spam based on how frequently these words appear in spam and non-spam emails.
    
    **Process**: The algorithm calculates the probability of the email being spam or non-spam based on the occurrence of these words, choosing the class with the highest probability.

### 2. **Support Vector Machines (SVM)**

**Support Vector Machines (SVM)** is a supervised learning algorithm used for classification tasks. In NLP, it is widely used for tasks like text classification, sentiment analysis, and named entity recognition. SVM works by finding a hyperplane that best separates data points of different classes.

-   **Example**:
    
    -   **Task**: Sentiment analysis of movie reviews.
    -   SVM uses features like word frequency (e.g., "good," "bad," "excellent") to classify movie reviews into positive or negative sentiment.
    
    **Process**: The algorithm searches for the optimal hyperplane that maximally separates positive and negative reviews in the feature space, based on the selected word features.

### 3. **Decision Trees**

**Decision Trees** are algorithms that make predictions by splitting data into branches based on feature conditions. In NLP, decision trees can be used for tasks like sentiment analysis and information extraction.

-   **Example**:
    
    -   **Task**: Classifying customer reviews as "positive" or "negative."
    -   The decision tree might first check if words like "love" or "great" are present in the review. If they are, the review is classified as positive; otherwise, the tree checks for other keywords like "bad" or "terrible" to classify it as negative.
    
    **Process**: A series of "if-else" conditions guide the tree to classify the text into the appropriate category.

### 4. **Random Forests**

**Random Forests** is an ensemble learning method that builds multiple decision trees and combines their results to improve accuracy and reduce overfitting. In NLP, random forests can be used for tasks like text classification and named entity recognition.

-   **Example**:
    
    -   **Task**: Identifying named entities (e.g., people, organizations, locations) in a text.
    -   A random forest model would analyze various features (word position, capitalization, and neighboring words) to predict whether a word is an entity or not.
    
    **Process**: Multiple decision trees are built, each with a subset of features and data, and their results are combined to produce the final prediction.

### 5. **Recurrent Neural Networks (RNN)**

**Recurrent Neural Networks (RNN)** are neural networks that excel at sequence-based tasks like language modeling, machine translation, and sentiment analysis. RNNs process each word in a sentence in sequence and maintain a hidden state that helps capture temporal dependencies and context within the sequence.

-   **Example**:
    
    -   **Task**: Predicting the next word in a sentence.
    -   In a sentence like "I am going to the," an RNN might predict the next word to be "store" based on the preceding words.
    
    **Process**: The RNN processes each word in the sentence one by one, and the hidden state is updated with each new word, capturing the sequence context.
   

### 6. **Long Short-Term Memory (LSTM)**

**LSTMs** are a type of RNN designed to overcome the **vanishing gradient problem** by capturing both short-term and long-term dependencies in sequences. LSTMs are particularly useful in applications like machine translation, named entity recognition, and text generation.

-   **Example**:
    
    -   **Task**: Machine translation (e.g., translating English to French).
    -   LSTM networks can remember long sequences and translate "I am going to the store" as "Je vais au magasin" by maintaining context across the sequence of words.
    
    **Process**: LSTM uses special gates (forget, input, output) to retain or discard information in the sequence, allowing it to capture long-range dependencies.

### 7. **Transformer Networks**

**Transformers** are a relatively recent architecture that has revolutionized NLP. They use **self-attention mechanisms** to capture the relationships between words, allowing for parallel processing and better handling of long-range dependencies. Transformers have led to the development of models like **BERT** and **GPT**, which achieve state-of-the-art performance in various NLP tasks.

-   **Example**:
    
    -   **Task**: Named entity recognition (NER) using **BERT**.
    -   Given a sentence like "Barack Obama was the president of the United States," BERT can recognize "Barack Obama" as a person and "United States" as a location by analyzing the context of each word.
    
    **Process**: Transformers use self-attention to weigh the importance of each word in a sentence relative to others, allowing the model to capture contextual information across long sequences.

## Question 23

**What is Sequence Labelling in NLP?**

Sequence labelling is one of the fundamental NLP tasks in which, categorical labels are assigned to each individual element in a sequence. The sequence can represent various linguistic units such as words, characters, sentences, or paragraphs.

Sequence labelling in NLP includes the following tasks.

-   Part-of-Speech Tagging (POS Tagging): In which part-of-speech tags (e.g., noun, verb, adjective) are assigned to each word in a sentence.
-   Named Entity Recognition (NER): In which named entities like person names, locations, organizations, or dates are recognized and tagged in the sentences.
-   Chunking: Words are organized into syntactic units or “chunks” based on their grammatical roles (for example, noun phrase, verb phrase).
-   Semantic Role Labeling (SRL): In which, words or phrases in a sentence are labelled based on their semantic roles like Teacher, Doctor, Engineer, Lawyer etc
-   Speech Tagging: In speech processing tasks such as speech recognition or phoneme classification, labels are assigned to phonetic units or acoustic segments.

Machine learning models like Conditional Random Fields (CRFs), Hidden Markov Models (HMMs), recurrent neural networks (RNNs), or transformers are used for sequence labelling tasks. These models learn from the labelled training data to make predictions on unseen data.


## Question 24

**What is topic modelling in NLP?**

Topic modelling is Natural Language Processing task used to discover hidden topics from large text documents. It is an unsupervised technique, which takes unlabeled text data as inputs and applies the probabilistic models that represent the probability of each document being a mixture of topics. For example, A document could have a 60% chance of being about neural networks, a 20% chance of being about Natural Language processing, and a 20% chance of being about anything else.

Where each topic will be distributed over words means each topic is a list of words, and each word has a probability associated with it. and the words that have the highest probabilities in a topic are the words that are most likely to be used to describe that topic. For example, the words like “neural”, “RNN”, and “architecture” are the keywords for neural networks and the words like ‘language”, and “sentiment” are the keywords for Natural Language processing.

There are a number of topic modelling algorithms but two of the most popular topic modelling algorithms are as follows:

-   [****Latent Dirichlet Allocation (LDA)****](https://www.geeksforgeeks.org/latent-dirichlet-allocation)****:**** LDA is based on the idea that each text in the corpus is a mash-up of various topics and that each word in the document is derived from one of those topics. It is assumed that there is an unobservable (latent) set of topics and each document is generated by Topic Selection or Word Generation.
-   [****Non-Negative Matrix Factorization (NMF)****](https://www.geeksforgeeks.org/non-negative-matrix-factorization)****:**** NMF is a matrix factorization technique that approximates the term-document matrix (where rows represent documents and columns represent words) into two non-negative matrices: one representing the topic-word relationships and the other the document-topic relationships. NMF aims to identify representative topics and weights for each document.

Topic modelling is especially effective for huge text collections when manually inspecting and categorising each document would be impracticable and time-consuming. We can acquire insights into the primary topics and structures of text data by using topic modelling, making it easier to organise, search, and analyse enormous amounts of unstructured text.


### Example of Topic Modelling

Let’s say you have a collection of 1000 articles on different machine learning subjects, including neural networks, NLP, and deep learning. Topic modelling might identify the following topics:

1.  **Topic 1 (Neural Networks)**: Words like "neural," "RNN," "architecture," "training."
2.  **Topic 2 (Natural Language Processing)**: Words like "language," "text," "parsing," "sentiment."
3.  **Topic 3 (Deep Learning)**: Words like "deep," "layers," "CNN," "training."

For a particular document, topic modelling might output:

-   60% chance it’s about neural networks
-   30% chance it’s about deep learning
-   10% chance it’s about NLP

Each document is a mixture of these topics in varying proportions.

### Topic Modelling Algorithms

Two of the most commonly used algorithms for topic modelling are:

#### 1. **Latent Dirichlet Allocation (LDA)**

**LDA** assumes that each document is composed of multiple topics, and each topic is a distribution over words. The algorithm works by assigning each word in a document to a particular topic based on probabilities. LDA attempts to identify **latent (hidden)** topics by examining patterns of word co-occurrence across documents.

-   **How it works**:
    -   LDA iterates between assigning words in each document to topics and refining the probability distributions of topics over words.
    -   It assumes that documents have multiple topics and generates each word based on a topic selection.For example, LDA might assign "neural," "RNN," and "backpropagation" to the "Neural Networks" topic and "language," "syntax," and "grammar" to the "NLP" topic.

#### 2. **Non-Negative Matrix Factorization (NMF)**

**NMF** is a matrix factorization technique that decomposes a term-document matrix (representing the frequency of words in documents) into two non-negative matrices:

-   **Document-topic matrix**: Describes the contribution of each topic to each document.
    
-   **Topic-word matrix**: Describes the contribution of each word to each topic.
    
-   **How it works**:
    
    -   NMF identifies topics by finding groups of words that frequently appear together across documents.
    -   The two resulting matrices describe the topics and how they relate to both the documents and the words.
    
    For example, if NMF is applied to a collection of articles, it will produce a list of topics, each associated with specific words. One topic might focus on "neural networks" with words like "neuron," "RNN," and "activation."


## Question 25

**What is the GPT?**

[GPT](https://www.geeksforgeeks.org/gpt-4-vs-gpt-3) stands for “Generative Pre-trained Transformer”. It refers to a collection of large language models created by OpenAI. It is trained on a massive dataset of text and code, which allows it to generate text, generate code, translate languages, and write many types of creative content, as well as answer questions in an informative manner. The GPT series includes various models, the most well-known and commonly utilised of which are the GPT-2 and GPT-3.

GPT models are built on the Transformer architecture, which allows them to efficiently capture long-term dependencies and contextual information in text. These models are pre-trained on a large corpus of text data from the internet, which enables them to learn the underlying patterns and structures of language.

### Explain
#### Key Features of GPT:
1.  **Pre-training**: The model is first pre-trained on a massive corpus of publicly available text data, such as books, articles, and websites. This allows GPT to learn the underlying patterns, structures, and knowledge in language.
    
2.  **Generative**: Once trained, GPT can generate text that looks like it was written by a human. Given an initial prompt or starting sentence, GPT continues writing, producing full paragraphs, stories, essays, or responses.
    
3.  **Transformer Architecture**: GPT leverages the **Transformer model**, which uses self-attention mechanisms to understand context and dependencies between words. This allows GPT to excel at tasks that require a deep understanding of context and structure, such as text completion and translation.
    
4.  **Fine-tuning**: While GPT is pre-trained on general text data, it can be fine-tuned on specific tasks (e.g., customer service, medical questions) to adapt to specialized use cases.


## Question 26

**What are word embeddings in NLP?**

[Word embeddings](https://www.geeksforgeeks.org/word-embeddings-in-nlp) in NLP are defined as the dense, low-dimensional vector representations of words that capture semantic and contextual information about words in a language. It is trained using big text corpora through unsupervised or supervised methods to represent words in a numerical format that can be processed by machine learning models.

The main goal of Word embeddings is to capture relationships and similarities between words by representing them as dense vectors in a continuous vector space. These vector representations are acquired using the distributional hypothesis, which states that words with similar meanings tend to occur in similar contexts. Some of the popular pre-trained word embeddings are Word2Vec, GloVe (Global Vectors for Word Representation), or FastText. The advantages of word embedding over the traditional text vectorization technique are as follows:

-   It can capture the Semantic Similarity between the words
-   It is capable of capturing syntactic links between words. Vector operations such as “king” – “man” + “woman” may produce a vector similar to the vector for “queen,” capturing the gender analogy.
-   Compared to one-shot encoding, it has reduced the dimensionality of word representations. Instead of high-dimensional sparse vectors, word embeddings typically have a fixed length and represent words as dense vectors.
-   It can be generalized to represent words that they have not been trained on i.e. out-of-vocabulary words. This is done by using the learned word associations to place new words in the vector space near words that they are semantically or syntactically similar to.

### Example of Word Embeddings

Let’s take an example to illustrate how word embeddings capture relationships between words.

Assume we have the following words: **king**, **queen**, **man**, and **woman**. Using word embeddings, these words can be represented as vectors in a high-dimensional space, like this:

-   **king** → [0.5, 0.8, -0.1, ...]
-   **queen** → [0.4, 0.9, -0.2, ...]
-   **man** → [0.2, 0.7, 0.1, ...]
-   **woman** → [0.3, 0.6, 0.0, ...]

One of the key advantages of word embeddings is that **vector operations** on these embeddings can capture relationships. For example, the vector difference between **king** and **man** can be similar to the vector difference between **queen** and **woman**:

$$\text{king} - \text{man} + \text{woman} \approx \text{queen}$$

This operation shows that the model understands the relationship between gender and royalty, capturing analogies like **"king is to man as queen is to woman"**.


## 🌟 Question 27

**What are the various algorithms used for training word embeddings?**

There are various approaches that are typically used for training word embeddings, which are dense vector representations of words in a continuous vector space. Some of the popular word embedding algorithms are as follows:

-   [****Word2Vec****](https://www.geeksforgeeks.org/python-word-embedding-using-word2vec): Word2vec is a common approach for generating vector representations of words that reflect their meaning and relationships. Word2vec learns embeddings using a shallow neural network and follows two approaches: CBOW and Skip-gram
    -   CBOW (Continuous Bag-of-Words) predicts a target word based on its context words.
    -   Skip-gram predicts context words given a target word.
-   ****GloVe****: GloVe (Global Vectors for Word Representation) is a word embedding model that is similar to Word2vec. GloVe, on the other hand, uses objective function that constructs a co-occurrence matrix based on the statistics of word co-occurrences in a large corpus. The co-occurrence matrix is a square matrix where each entry represents the number of times two words co-occur in a window of a certain size. GloVe then performs matrix factorization on the co-occurrence matrix. Matrix factorization is a technique for finding a low-dimensional representation of a high-dimensional matrix. In the case of GloVe, the low-dimensional representation is a vector representation for each word in the corpus. The word embeddings are learned by minimizing a loss function that measures the difference between the predicted co-occurrence probabilities and the actual co-occurrence probabilities. This makes GloVe more robust to noise and less sensitive to the order of words in a sentence.
-   [****FastText****](https://www.geeksforgeeks.org/fasttext-working-and-implementation): FastText is a Word2vec extension that includes subword information. It represents words as bags of character n-grams, allowing it to handle out-of-vocabulary terms and capture morphological information. During training, FastText considers subword information as well as word context..
-   [****ELMo****](https://www.geeksforgeeks.org/overview-of-word-embedding-using-embeddings-from-language-models-elmo): ELMo is a deeply contextualised word embedding model that generates context-dependent word representations. It generates word embeddings that capture both semantic and syntactic information based on the context of the word using bidirectional language models.
-   [****BERT****](https://www.geeksforgeeks.org/explanation-of-bert-model-nlp): A transformer-based model called BERT (Bidirectional Encoder Representations from Transformers) learns contextualised word embeddings. BERT is trained on a large corpus by anticipating masked terms inside a sentence and gaining knowledge about the bidirectional context. The generated embeddings achieve state-of-the-art performance in many NLP tasks and capture extensive contextual information.


### Explain 
### 1. Word2Vec
**Word2Vec** is one of the most widely used algorithms for generating word embeddings. It uses a shallow neural network to learn vector representations of words by considering the context in which words appear. Word2Vec has two main approaches:

- **CBOW (Continuous Bag of Words)**:
  - CBOW predicts the target word based on the context words surrounding it.
  - **Example**: Given the context words "**The __ is running,**" the model predicts the missing word "**dog**."
  
- **Skip-gram**:
  - Skip-gram predicts the context words given the target word.
  - **Example**: Given the target word "**dog**," the model predicts the context words "**The**" and "**running**."

The resulting embeddings from Word2Vec capture the semantic relationships between words. For example, the model might learn that words like "**king**" and "**queen**" have similar relationships to "**man**" and "**woman**."

**Example**:  
Suppose the model is trained on the sentence:

- "**The dog chased the ball.**"

With **CBOW**, the model might learn the relationship between "**dog**" and the context words "**chased**" and "**ball**." With **Skip-gram**, the model would predict "**chased**" and "**ball**" given the word "**dog**."

### 2. GloVe (Global Vectors for Word Representation)
**GloVe** is another popular algorithm for generating word embeddings, but it approaches the problem differently from Word2Vec. GloVe focuses on the global word co-occurrence statistics in the corpus.

- GloVe builds a **co-occurrence matrix** where each entry represents how frequently two words co-occur within a specific window size in the text.
- It then performs **matrix factorization** on this co-occurrence matrix to obtain word embeddings.

This approach captures the relationships between words by learning from the overall distribution of words in the corpus, rather than relying on the local context of words like Word2Vec.

**Example**:  
Consider a corpus where the word "**cat**" frequently co-occurs with "**pet**" and "**animal**." GloVe learns embeddings where "**cat**," "**pet**," and "**animal**" are represented close together in the vector space.

**Co-occurrence matrix**:

|         | cat | pet | animal |
|---------|-----|-----|--------|
| **cat** | 10  | 5   | 7      |
| **pet** | 5   | 10  | 8      |
| **animal** | 7 | 8  | 10     |

After matrix factorization, the words "**cat**," "**pet**," and "**animal**" will have similar embeddings, representing their shared meaning.

### 3. FastText
**FastText** is an extension of Word2Vec developed by Facebook, which improves upon the handling of **out-of-vocabulary (OOV)** words by incorporating subword information.

- FastText breaks down words into **n-grams** (subword units), which allows it to generate embeddings for words that weren't seen during training by composing them from subwords.
- This is useful for morphologically rich languages, where words may take many forms due to conjugation or inflection.

**Example**:  
Suppose the word "**unbelievable**" is not present in the training corpus. FastText can break this word into subwords like:

- "**un-**", "**believe**", "**-able**"

FastText uses the embeddings of these subwords to construct a vector for "**unbelievable**," placing it near similar words like "**amazing**" and "**incredible**" in the embedding space, even if the word itself was never seen in the corpus.

### 4. ELMo (Embeddings from Language Models)
**ELMo** generates **contextualized word embeddings**, meaning that the word embeddings are dependent on the **context** in which the word appears. Unlike Word2Vec and GloVe, which generate a single static embedding for each word, ELMo generates different embeddings for a word based on the sentence.

- ELMo uses **bidirectional language models (bi-LSTMs)** to capture both semantic and syntactic information from the entire sentence.

**Example**:  
Consider the word "**bank**" in two different sentences:

1. "**I deposited money in the bank.**"
2. "**I sat by the river bank.**"

ELMo generates different embeddings for "**bank**" in these two sentences based on the context. In sentence 1, "**bank**" refers to a financial institution, while in sentence 2, it refers to the side of a river.

### 5. BERT (Bidirectional Encoder Representations from Transformers)
**BERT** is a **transformer-based** model that generates **deeply contextualized word embeddings**. BERT learns word embeddings by processing the entire sentence in **both directions** (left-to-right and right-to-left), capturing a word's meaning based on its **bidirectional context**.

- BERT is trained using a **masked language model (MLM)**, where certain words in a sentence are masked, and the model learns to predict the masked words by understanding the context.
- BERT embeddings are state-of-the-art for many NLP tasks, such as **text classification**, **question answering**, and **named entity recognition**.

**Example**:  
Consider the sentence:

- "**The teacher taught the students.**"

If BERT is asked to predict the word "**taught**" from the masked sentence "**The teacher [MASK] the students,**" it learns a representation of "**taught**" by considering the bidirectional context of both "**The teacher**" and "**the students**." This allows BERT to understand the precise meaning of the word in context.

### Summary of Algorithms:

| **Algorithm** | **Key Approach** | **Context Dependency** | **Example Use Case**                      |
|---------------|------------------|------------------------|-------------------------------------------|
| **Word2Vec**  | Neural network-based, CBOW & Skip-gram | Static (same embedding for all contexts) | Text classification, sentiment analysis  |
| **GloVe**     | Co-occurrence matrix and matrix factorization | Static | Information retrieval, topic modeling     |
| **FastText**  | Subword-based (n-grams) | Static | Handling OOV words, morphologically rich languages |
| **ELMo**      | Bi-LSTM-based contextualized embeddings | Contextual (varies by sentence) | Named entity recognition, machine translation |
| **BERT**      | Transformer-based bidirectional embeddings | Deeply contextual (varies by sentence) | Question answering, text summarization  |

Each algorithm offers different advantages depending on the task, data, and whether **contextual understanding** or **out-of-vocabulary handling** is required. Models like **BERT** and **ELMo** capture deep contextual information, while models like **Word2Vec**, **GloVe**, and **FastText** are more efficient for general word embeddings.


## Question 28

**How to handle out-of-vocabulary (OOV) words in NLP?**

OOV words are words that are missing in a language model’s vocabulary or the training data it was trained on. Here are a few approaches to handling OOV words in NLP:

1.  ****Character-level models:**** Character-level models can be used in place of word-level representations. In this method, words are broken down into individual characters, and the model learns representations based on character sequences. As a result, the model can handle OOV words since it can generalize from known character patterns.
2.  ****Subword tokenization:**** Byte-Pair Encoding (BPE) and WordPiece are two subword tokenization algorithms that divide words into smaller subword units based on their frequency in the training data. This method enables the model to handle OOV words by representing them as a combination of subwords that it comes across during training.
3.  ****Unknown token:**** Use a special token, frequently referred to as an “unknown” token or “UNK,” to represent any OOV term that appears during inference. Every time the model comes across an OOV term, it replaces it with the unidentified token and keeps processing. The model is still able to generate relevant output even though this technique doesn’t explicitly define the meaning of the OOV word.
4.  ****External knowledge:**** When dealing with OOV terms, using external knowledge resources, like a knowledge graph or an external dictionary, can be helpful. We need to try to look up a word’s definition or relevant information in the external knowledge source when we come across an OOV word.
5.  ****Fine-tuning:**** We can fine-tune using the pre-trained language model with domain-specific or task-specific data that includes OOV words. By incorporating OOV words in the fine-tuning process, we expose the model to these words and increase its capacity to handle them.

### Explain 
### 1. **Character-Level Models**

**Character-level models** break down words into individual characters, allowing the model to learn representations based on character sequences instead of whole words. This enables the model to generalize to OOV words since it processes each word as a sequence of characters, regardless of whether it has seen the word before.

#### Example:

Suppose the word **“supercalifragilisticexpialidocious”** is an OOV word. A character-level model would process it as a sequence of characters:

-   `["s", "u", "p", "e", "r", "c", "a", ...]`

Even though this word wasn't part of the training data, the model can learn patterns and relationships between individual characters and generate an embedding based on the character sequence, allowing it to handle long or unfamiliar words.

### 2. **Subword Tokenization**

**Subword tokenization** algorithms like **Byte-Pair Encoding (BPE)** and **WordPiece** split words into smaller subword units based on their frequency in the training data. This technique enables the model to handle OOV words by breaking them down into familiar subword pieces and recombining them during inference.

#### Example:

Consider the OOV word **“unbelievable.”**

-   **BPE** might break it into subwords like: `["un", "believe", "able"]`.

Even if the full word **“unbelievable”** wasn’t seen during training, the subwords **“un”**, **“believe”**, and **“able”** were likely seen, allowing the model to handle the word by combining these subwords to infer its meaning.

-   Similarly, **WordPiece** would break the word into familiar subword units like: `["un", "##believable"]`.

### 3. **Unknown Token (UNK)**

In cases where a model encounters an OOV word, it can replace the word with a special **unknown token (UNK)**. This approach does not attempt to learn a representation for the OOV word itself, but instead uses the **UNK token** as a placeholder during processing.

#### Example:

If the model encounters an OOV word like **"quizzaciously"**, it will replace it with an **UNK token** during inference, and the sentence may become:

-   "**The student answered UNK.**"

While this approach is simple, it doesn't capture the semantics of the OOV word and may reduce the model's overall performance in tasks that require precise understanding of specific words.

### 4. **External Knowledge**

In some cases, **external knowledge sources** such as dictionaries, knowledge graphs, or APIs can be used to look up the meaning or context of an OOV word, providing the model with additional information to handle unfamiliar terms.

#### Example:

If the model encounters the OOV word **“CRISPR”** (a term in genetic engineering), the model could query an external knowledge graph or dictionary to retrieve the definition:

-   **"CRISPR: A gene-editing technology that allows for precise, targeted changes to the genome."**

By incorporating this external knowledge, the model can handle domain-specific terms like **“CRISPR”** even if it wasn't part of the training corpus.

### 5. **Fine-tuning on Domain-Specific Data**

Fine-tuning a pre-trained language model on domain-specific or task-specific data that contains OOV words can improve the model's ability to handle new terms. By exposing the model to these words during fine-tuning, the model adapts to handle these OOV terms in future tasks.

#### Example:

Suppose a pre-trained model was trained on general text data and now needs to work with medical terminology (e.g., **"angioplasty"** or **"tachycardia"**). Fine-tuning the model on a medical corpus will expose it to these OOV terms, enabling it to better handle domain-specific language.


## Question 29

**What is the difference between a word-level and character-level language model?**

The main difference between a word-level and a character-level language model is how text is represented. A character-level language model represents text as a sequence of characters, whereas a word-level language model represents text as a sequence of words.

Word-level language models are often easier to interpret and more efficient to train. They are, however, less accurate than character-level language models because they cannot capture the intricacies of the text that are stored in the character order. Character-level language models are more accurate than word-level language models, but they are more complex to train and interpret. They are also more sensitive to noise in the text, as a slight alteration in a character can have a large impact on the meaning of the text.

The key differences between word-level and character-level language models are:


|                    | **Word-level**                                          | **Character-level**                                     |
|----------------------------------|--------------------------------------------------------|--------------------------------------------------------|
| **Text representation**          | Sequence of words                                      | Sequence of characters                                 |
| **Interpretability**             | Easier to interpret                                    | More difficult to interpret                            |
| **Sensitivity to noise**         | Less sensitive                                         | More sensitive                                         |
| **Vocabulary**                   | Fixed vocabulary of words                              | No predefined vocabulary                               |
| **Out-of-vocabulary (OOV) handling** | Struggles with OOV words                              | Naturally handles OOV words                            |
| **Generalization**               | Captures semantic relationships between words          | Better at handling morphological details               |
| **Training complexity**          | Smaller input/output space, less computationally intensive | Larger input/output space, more computationally intensive |
| **Applications**                 | Well-suited for tasks requiring word-level understanding | Suitable for tasks requiring fine-grained details or morphological variations |



## Question 30

**What is word sense disambiguation?**

The task of determining which sense of a word is intended in a given context is known as [word sense disambiguation (WSD)](https://www.geeksforgeeks.org/word-sense-disambiguation-in-natural-language-processing). This is a challenging task because many words have several meanings that can only be determined by considering the context in which the word is used.

For example, the word “bank” can be used to refer to a variety of things, including “a financial institution,” “a riverbank,” and “a slope.” The term “bank” in the sentence “I went to the bank to deposit my money” should be understood to mean “a financial institution.” This is so because the sentence’s context implies that the speaker is on their way to a location where they can deposit money.

## Reference
- https://www.geeksforgeeks.org/nlp-interview-questions/

