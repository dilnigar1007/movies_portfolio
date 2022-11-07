# movies_portfolio

### first step of cleaning the data:
In this section, our group first converted tsv files we downloaded from Kaggle to csv file. In the first code, I imported "titles-ratings.csv" file to read in all the data we have. Next, sorted them by averagerating column, so we get the first ten or top ten movies in this dataset. I created a new dataframe based on this sorted data and only kept this 10 movies. In the next step of this data cleaning, we will be combining "title-metadata.csv" and this new data "topten_movies.csv" using SQL. Since we both have "tconst" columns in both datasets, we can join them and gather movies titles using this mutual column. 
