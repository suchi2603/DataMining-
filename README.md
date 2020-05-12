# DataMining Project
The project is on predicting the ratings of BoardGameGeek Reviews
The dataset is available at: https://www.kaggle.com/jvanelteren/boardgamegeek-reviews.

The dataset contains three separate CSV files:

* The first CSV file named 20119-05-02 contain more precisis information for each game the game rank, year, number of users rated etc.

* bgg_13m_reviews CSV file has all reviews stored in it.

* games_details_info has the specific details about the data. 

In the dataset, all categories have unique ranks for each game, except the leading board game ranking.

In the dataset, all categories have unique ranks for each game, except the leading board game ranking.

The majority of the 15 categories only have one board game, except abstract, children, customizable, family, party, strategy, thematic, and war.

All numerical variables excluding categories have no null values.


-> *The goal of the project is to predict the rating of the review, and the main thing that should be highlighted is the kind of improvement done over the given available codes and tutorials online.*

As per my progress, 

I a beginner in Data Analysis and using Python programming so I preferred first to explore the complete dataset clearly using various libraries and inbuilt functions provided by python packages.

# Explaining the process

 The three datasets are imported using the "python read_csv", an important pandas function to read csv files and do operations on it.

  * The head() function is used to get the first n rows of the required dataframe which was imported using pandas.

  * The data types that are present in the data can be known using the ".dtype".
  
  * The describe() funtion allows us to know about the Mean, Standard Deviation, Count, Min, Max etc.
  
  * ".isna().sum()" is very useful to know if there are any NULL or NaN values present in the datasets so that it would help in further process.
  
Therefore, I have performed analysis and could view the datatypes, shape of the data, the complete description like the Mean of the required columns.  

## Visualizing data

Data visualization is very helpful tool in understanding the data better in lesser time. Anyone from a any background can easily be able to undestand the concepts when it is explained through pictorail ways.

visualization of data can be easy with python using:

  * *Pandas* 
  
  * *Matplotlib*
  
  * *Seaborn*
  
  * *ggplot*
  
  * *Plotly etc*

A heatmap which was looking quite attractive which can be a best diagramatic description of the data present in games_details_info.csv file.  
  
I used Histograms to show the visual relationship between various columns present in the data.

 a) Firstly, the "Year" column of the first dataset is plotted.

 b) Later the "average", "Bayes average" and "User ratings" columns were also plotted.

Under the data visualization we have "seaborn" in python for a great visualization of data.

Using "seaborn" we can create a custom diverging colour map. Here I used 'GnBu' colour but various other colours like 'Cool', 'cool_r', 'copper', 'GuBn' etc can be used.

## Merging the columns
Once we look at the data sets, there are columns that are common in the datasets and so we can mannage merging the repeating columns to improve execution time.

The code for merging the selected coumns of a given dataset is executed. For example the column like "Average" is available in both the datasets but one has a precision of one decimal point and the other has a precision of three. so if we merge them it is easier to understand the values and consider whichever is needed.

## Descriptive analysis of BoardGames

1) The top 50 words that appear are plotted using the WordCloud and also listed

Text Preprocessing is done before for:
  * Sorting words in reverse order
  * Deleting the less frequency words from the list
  * and Finally generating the bag of Words
For now, the Word cloud is plotted with 250 most frequent words with a black background. 

2) Top 25 reviews of the data have been displayed using  Barplot.

3)Correlation is one of the important aspects for representing the numerical values of the target rating.This has also been done.

4)Plot for maximum number of games published durimg the years 2010 to 2018 was plotted.


For any given dataset, the description is really very important to understand what exactly the data is holding. For performing any other futher steps the analysis of the dataset is the next important step to be done.

 maximum number of board games published during a given duration was also helpful for us to know aboutthe year in which there were a lot of games published.

## Concludings
From the analysis of the data is concluded that, maximum number of board games published was during 2016. This is depicted using the plot of curve.

There were also the list of all top frequency words like 'game', 'play, 'it', 'fun' etc.

The most reviewed Board game was the 'carcassonne' and these can be seen from the Histogram plotted.

