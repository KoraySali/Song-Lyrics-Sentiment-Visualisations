# Song-Lyrics-Sentiment-Visualisations
# Description:

The provided Python code demonstrates a text analysis pipeline that involves cleaning and processing song lyrics data, performing sentiment analysis, and visualising the results. The code leverages various libraries, including NLTK, Pandas, Gensim, and AFINN, to perform these tasks. Here's a breakdown of the technical details:

* Data Preparation:
The code starts by importing necessary libraries like NLTK, Pandas, and Gensim.
It identifies a folder containing song lyrics text files and creates a list of file paths for these lyrics.

* Text Cleaning:
A regular expression pattern is defined to remove non-alphanumeric characters from the song lyrics.
The code iterates through each file, reads its content, and cleans it by removing unwanted characters. It then overwrites the original file with the cleaned text.

* Data Loading and Structuring:
The code reads the cleaned text files and organises the data into a Pandas DataFrame, making it easier to work with structured data.

* Text Processing:
The song lyrics are tokenised into individual words using NLTK's word_tokenize function, and the tokenised words are stored in a new column.

* Metadata Assignment:
The code assigns gender and date of birth (DOB) information to the artists based on their filenames. This metadata is stored in separate DataFrame columns.

* Text Analysis:
Text data is lemmatised using NLTK's WordNetLemmatizer, improving the quality of the text for analysis.

![](https://github.com/KoraySali/Song-Lyrics-Sentiment-Visualisations/blob/main/Frequency%20of%20the%20word%20love%20per%20artist.png?raw=true)

* Sentiment Analysis:
AFINN sentiment analysis is applied to the lemmatised words to calculate sentiment scores for each word. These scores are stored in a new column.

![](https://github.com/KoraySali/Song-Lyrics-Sentiment-Visualisations/blob/main/Wordcloud%20.png?raw=true)

* Positive and Negative Words:
The code identifies positive and negative words based on their sentiment scores and stores them in separate DataFrame columns.

![](https://github.com/KoraySali/Song-Lyrics-Sentiment-Visualisations/blob/main/Average%20sentiment%20score%20of%20an%20artist%20distributed%20by%20gender.png?raw=true)

* Topic Modelling:
Gensim's LDA model is employed to discover topics within the text data. The code creates a dictionary and corpus for the words and applies LDA to reveal topics.

* Data Visualisations:
The code generates various data visualisations, including word clouds representing topics, a pie chart showing the distribution of artists by gender, bar charts indicating word frequency and sentiment scores, and more.

![](https://github.com/KoraySali/Song-Lyrics-Sentiment-Visualisations/blob/main/Average%20sentiment%20score%20of%20an%20artist.png?raw=true)
