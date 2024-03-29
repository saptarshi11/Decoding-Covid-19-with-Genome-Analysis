# Decoding-Covid-19-with-Genome-Analysis

WORKFLOW OF MY NOTEBOOK 1: (Covid19-CORD-NER)
Text Cleaning and Preprocessing:
•	First, imported 10000 rows from the json file (“CORD-NER-full.json”). 
•	Converted the json data to csv and imported it.
•	Searched for articles published in the year 2020.
•	Dropped articles with missing abstract.
•	Dropped articles with duplicate abstract.
•	In abstract column:
-	Converted text to lowercase.
-	Removed non-English words.
-	Removed Stopwords.
-	Removed words with single characters.
•	Inverted index
Article Matching and Deep Cleaning:
•	Developing a keyword list that would facilitate a search to locate only applicable articles.
•	Took data from required website articles and saved the index location in a new data frame.
•	It uses lemmatization and POS tagging in order to provide unambiguous information.
•	The word cloud was created to realize which words or phrases were surprisingly recurring.
Topic Extraction
________________________________________
•	The LDA model has been built to explore topics and the c_v model features coherence measure.
•	Checked perplexity of my LDA Model
•	Thematically relevant sentences are huge technological bypasses.
LDA visualization.
•	On each theme of the document, different bars will be used to illustrate the data visually.
•	T-SNE:
Document topic matrix generated.
Multi-dimensionally clustering of LDA topic based on T-SNE.
Semantic-Based Search:

•	Such data as those with duplicates or missing values.
•	Dropping non-English articles.
•	Spacy Parser and Tokenizer are a regex based library models that are task oriented in their nature.
•	Sentence Tokenization
•	Word2vec Training
•	Ranking documents
•	Storing the model and the dataframe as a variable is what we are saving here.






WORKFLOW OF MY NOTEBOOK 2: 
(COVID-19-CORD-NER- information-extraction- Question-Answering)
1.	NER Extraction from Text
2.	Dependency parses
3.	Question-Answering
NER Extraction from Text:
•	spaCy based imports
•	NER extraction using Spacy library
•	Closer look at what spaCy is doing when it performs named entity recognition
•	Finding same entity texts
Dependency parses:
•	Encoding grammatical information by using spaCy's dependency visualizer.
•	Identifying verbs + direct objects that are grammatically linked to a location.
•	Identifying all the actions related to a single city, Wuhan.
•	Top 10 Geopolitical Entities Related to "Origin", "Case", or "Transmission.

Question-Answering:
•	Downloaded a transformer model that's already been trained on SQuAD from the 
Huggingface model repository.
•	Performed queries
