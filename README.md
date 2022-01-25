##### A Python script to analyze customer sentiment in NPS surveys.

## The problem

A common way to measure customer satisfaction with a service is the NPS (Net Promoter Score), which evaluates opinions in a 0 to 10 scale, classifying customers as Detractors (0 to 6), Passives (7 to 8) or Promoters (9 and 10). Such a survey is usually accompanied by some form of text commentary, asking for critics or suggestions to continuosly improve the service. So, along with analyzing the quantitative aspects of such a survey, the commentaries could also hold valuable insight on customers' thoughts, and will be the primary focus of this project.

This script takes commonly formatted survey data, applies some preprocessing for data cleaning and exploratory analysis to identify insights on the quantitative part of a NPS survey, and then proceeds to apply NLP (natural language processing) techniques on the commentary data, such as Lemmatisation (grouping inflected words into single items), removing punctuation and removing stopwords (words that do not add meaning to sentences), so that in the end a wordcloud with commonly used words, bigrams and trigrams (2 and 3-word associations, respectively) is plotted. With such data representation, a user can easily identify trends in customers thoughts, often confirming initial hypotheses or revealing tendencies which weren't yet thought of.

A fake data sample is included on the project, representing a fictitious education company, and was generated using random methods, so it shouldn't hold as much insight on processes as real data would.

The full report with code and results can be found here: https://filipeoliveira94.github.io/nps-nlp-script/

## References and Tools Used

This script was built using Python, with the common data science packages 'numpy', 'pandas' and 'matplotlib', along with more specific packages such as 'spacy' and 'nltk' for NLP, and 'wordcloud' for the end-result wordclouds.

The documentation for these packages can be found here:
1. [SpaCy pt-br](https://spacy.io/models/pt)
2. [NLTK](https://www.nltk.org/)
3. [Wordcloud - PyPI](https://pypi.org/project/wordcloud/)
