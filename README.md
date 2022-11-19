# movies_portfolio
### Background
As a group we decided to study the relationship between how people feel about movies and how the critics rate the movies. It's a valid idea because it shows the disconnection between people's opinions. One from a normal movie watcher's point of view compared to someone whose job is to rate the movies.  

### Motivation
We noticed that a lot of the movies that say they're good isn't good. So instead of wasting our time with average movies, we want a good movie we enjoy. 

### Questions to answer
Are the top 5 rated movies receiving positive comments from most viewers?

## Project outline:
### Understanding the topic and gather required information
Our group focused on the relationship between top-rated movies and comments on them. Sometimes Rotten Tomato rates are different than what people actually think about those, and we see a variety of comments on twitter and other social media sites. We have downloaded our datasets from Kaggle.com. To be precise and make it not too complicated, we are going to focus on the top 10 movies. We have a clear question to answer throughout this analysis. 
-Question: Are the top 10 rated movies receiving positive comments from most viewers?
### Data understanding
Our initial dataset contains the following columns (source: https://www.kaggle.com/datasets/riyapatel1697/imdb-official-movies-dataset?select=title-metadata.tsv)
-title.basics.tsv - Contains the following information for titles:
-tconst (string) - alphanumeric unique identifier of the title
-titleType (string) – the type/format of the title (e.g. movie, short, tvseries, tvepisode, video, etc)
-primaryTitle (string) – the more popular title / the title used by the filmmakers on promotional materials at the point of release
-originalTitle (string) - original title, in the original language
-isAdult (boolean) - 0: non-adult title; 1: adult title
-startYear (YYYY) – represents the release year of a title. In the case of TV Series, it is the series start year
-endYear (YYYY) – TV Series end year. ‘\N’ for all other title types
-runtimeMinutes – primary runtime of the title, in minutes
-genres (string array) – includes up to three genres associated with the title
-title.crew.tsv – Contains the director and writer information for all the titles in IMDb. Fields include:
-tconst (string) - alphanumeric unique identifier of the title
-directors (array of nconsts) - director(s) of the given title
-writers (array of nconsts) – writer(s) of the given title
-title.ratings.tsv – Contains the IMDb rating and votes information for titles
-tconst (string) - alphanumeric unique identifier of the title
-averageRating – weighted average of all the individual user ratings
-numVotes - number of votes the title has received

### Data preparation:
In addition to the dataset we got from Kaggle, we are currently working on Twitter API by creating an account. Once this is completed, we are using the NLP (Natural Language Processing) method to extract comments on those 10 movies based on the hashtag or keywords they used. For the first part of the cleaning, we are going to drop anything that’s not in the top 10 list, then look at the key variables for example, averageRating and title.ratings.tsv for each variable. Then, we will import our extracted data into this and create another dataframe based on this.
### Analysis and modeling:
In the next step, we’re going to decide on our important variable that we’re going to use for our analysis. 
### Visualization and presentation:
For this step, we will be using Tableu to create our visualizations/graphs to show our results, which we will be using for our presentation later on. In our presentation, we will be using graphs to show how and where we got our data, what codes we used to clean the data and create our models, how we worked through APIs to extract data from Twitter, and data validation. Lastly, we will have a section for data restriction and limitations. 
