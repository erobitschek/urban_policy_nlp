# urban_policy_nlp
Repo for NLP analysis of open text field input from sustainable development survey data.

## author: Emily Robitschek 
## contact: erobitschek@ethz.ch

# Data 

The dataset that will be used for this project comes from the Spatial and Urban Policy Research (SPUR) group at ETH. This group conducted a survey on attitudes towards urban densification policies across several large cities, including: Berlin, Chicago, Los Angeles, New York City, London and Paris. As a part of this survey, there is also an open text field answer to the question "If you would like, we would be very grateful if you could briefly describe here why you generally decided in favor of or against certain proposals". For the initial stage of this project, I will analyze the open text responses from this short answer field for the cities where the survey was conducted in English (Chicago, Los Angeles, New York City, and London). 

More information on the publicly available dataset at these links: 
    - general info (german): https://irl.ethz.ch/research/forschung/housing-situation.html
    - general info (english) with links to data briefs: https://spur.ethz.ch/research/housing-situation.html
    - dataset and codebook: https://www.research-collection.ethz.ch/handle/20.500.11850/513683

# Goal
The research question is: "Can the information from this text field be analyzed in a systematic way that shows a) concordance with some key elements assessed with the survey design and b) any new insights about why respondents respond the way they do?"

# Code
In the "code" folder, there are two notebooks (one more to be added once analysis is finalized): 
    1) survey_preprocess shows the process and rational behind the data preprocessing
    2) survey_wordcloud includes code to generate words clouds from subsets of the survey responses
    3) survey_topicmodel includes the topic modelling associated with this dataset
    4) survey_relatio extracts narratives from the text responses to complement the topic modelling approach
    5) survey_linearmodels will integrate the results from the topicmodel to see if a predictive model can be based upon the topic modelling (TBD)


# Other useful links and resources:

## Subject area
More on Urban Densification, with a focus on Switzerland:
https://www.ebp.ch/en/topics/space/urban-densification

## Tools
Spacy and nltk: 
- https://spacy.io/usage/visualizers
- https://pythonspot.com/nltk-stop-words/

Wordclouds
- used this site as a resource: https://www.datacamp.com/community/tutorials/wordcloud-python
- wordcloud package author's underlying generation process: https://peekaboo-vision.blogspot.com/2012/11/a-wordcloud-in-python.html
- wordcloud package: https://amueller.github.io/word_cloud/

Topic modelling: 
- https://medium.com/@kurtsenol21/topic-modeling-lda-mallet-implementation-in-python-part-1-c493a5297ad2 (useful info for preprocessing)
- https://www.machinelearningplus.com/nlp/topic-modeling-gensim-python/ (largely based on this approach)
- https://anaconda.org/anaconda/gensim
- https://anaconda.org/conda-forge/pyldavis
- https://medium.com/analytics-vidhya/topic-modeling-using-gensim-lda-in-python-48eaa2344920
- 

Narrative discovery: 
- relatio github: https://github.com/relatio-nlp/relatio
- relatio publication: https://arxiv.org/pdf/2108.01720.pdf
