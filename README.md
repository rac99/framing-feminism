# DH-412 History and the Digital 

By: Arthur, Ryan, and Thomas

Research Question: _How has feminism been framed in US newspapers from 1980 to 2009?_

This Github repository contains all of our code for the project, as well as the data generated for it. An explanation of the key parts of the repository are found below. A copy of our final rpeort is also viewable in the PDF.

## data/ folder

This folder contains all of the data that we would be using for analysis and/or further processing:
- .zip files of our .csv files of our raw data, and processed data for topic modelling and colocation (you would need to unzip the zip locally)
- the results of our nltk colocations, both as .csv and also .txt
- additional stopwords used in stopwords-en.txt 
- word weightings for our topic modelling results in tm_word_weights.txt
- some of the graphs/figures we used

There is also a subfolder, under data/sample_articles, which includes the full article of the sample articles we referenced in our report. 

## lda_models/ folder

This folder contains the visualized LDA Models as .html files on each decade, as well as for the New York Times and Pittsburgh Post-Gazette. Visualized with pyLDAvis library.

## 0_rtf_conversion.ipynb

convert the rtf files taken from Nexis Uni into a csv for later use as a Pandas dataframe.

## 1_pre_processing.ipynb

Pre-process our data that we converted, namely into a cleaned text csv for topic modelling and for colocation. The only difference between the two is that the colocated cleaned text was not lemmatized to maintain the actual word that it was, whereas for the purposes of topic modelling we lemmatized.

1.1_plot_information.ipynb includes just some more statistics of our data, and a plot 

## 2_nltk_colocates.ipynb

This is the file where we used the nltk collocation library to perform the colocates.

2.1_colocate_graphs.ipynb is where we made the bump plot to show the change of colocate rankings over the three decades. 

## 3_topic_modelling.ipynb

This is the topic modelling file which was used to run the LDA model on the three different decades, as well as the two separate newspapers. 