![microsoft logo](https://github.com/rustyb08/phase_1_project/blob/main/images/Microsoft_logo_(2012).svg.png?raw=true)
# Microsoft New Original Content

Author: Rusty Brown

## Overview

Microsoft has decided to start a new movie studio, but they don’t know anything about making movies or the current movie market.  I’ve been tasked with reviewing the data of recent movie for trends and provide insights and recommendations.  I was able to combine basic movie data (titles, runtime, and genre) from IMDB and budget and gross data from The Numbers.  When comparing genre information from the top 100 worldwide grossing films to production budgets and gross, trends began to develop.  Action and Adventure films are the most popular and highest grossing among the top films.  They are also the films with the highest production budgets.  I would recommend Microsoft create an Action, Adventure, Sci-Fi film and expect to spend $175-$245 million.

## Business Understanding

Nearly 700 movies are released every year (over the last decade) ranging cute, animated children’s movie all the way up to gruesome thrillers and everything in between.  Armed with only that information, it would be nearly impossible to know what type of film would be successful.  That’s exactly the positions Microsoft finds itself in.  My goal is to analyze the data currently in the film industry and answer three questions about current market and how they may affect budget and gross:
1.	What trends are there with the different genres?
2.	What type of budget can you expect?
3.	What kind of movie lengths are present in the top movies?

## The Data

The data was pulled from five sources (not all sources were used for this analysis).
- Box Office Mojo
- IMDB
- The Numbers
- Rotten Tomatoes
- TheMovieDB

The Rotten Tomatoes and TheMovieDB data were not used as ratings, reviews, and popularity were not a part of my analysis. 

IMDB is a very in-depth source of information, it not only contains basic information about the movie, but also detailed information about the actors, directors, and writers.  With the scope of this project, we will focus on the basic movie information (title, runtime, start year, and genres) for nearly 150,000 movies.

Box Office Mojo (BOM) and The Numbers (TN) have similar data as they both have domestic and foreign gross as well as the release date/year.  BOM also includes what movie studio released the film, which could give us more analytical data, but is outside the scope of this project. BOM has data for 3,387 titles but seems to be missing a significant amount of data from foreign gross.  TN has the same information, excluding the movie studio, but includes production budget.  TN also has data for 5,782 films and at a glance has no missing data.  I chose to use the “movie_basics” table from IMDB and The Numbers for the basis of this project.

## Analysis

After cleaning the data and merging out two files along the movie title and release year, to insure I wasn’t merging different movie with the same title, I was left with 1,541 movies.  And while I could analyze all this data, I wanted to focus on only the most successful films to provide Microsoft with the best opportunity for success.  I chose to pair the data down to the top 100 films based on worldwide gross.  We can see by looking at this data that the Action and Adventure genres are the most popular among these successful films.

![Genre Count](https://github.com/rustyb08/phase_1_project/blob/main/images/Genre_count.png?raw=true)

The most common range for production budget is $140-$185 million.  59% of the top grossing films have a budget of $140-$230 million.

![Production Budget](https://github.com/rustyb08/phase_1_project/blob/main/images/Production_budget.png?raw=true)

Also, while not a direct correlation, movies that are over 2 hours tend to have a higher gross than shorter films.

![Runtime](https://github.com/rustyb08/phase_1_project/blob/main/images/Runtime.png?raw=true)

## Conclusions

This analysis led me to three recommendations for the team at Microsoft’s new films studio:
- The Action and Adventure genres are by far the most popular and among the most lucrative.
- - Specifically, Action/Adventure/Sci-Fi which averaged a return on investment of $809 million among the top grossing films.
- Plan for a production budget of $185-$230 million.
- -	The Action/Adventure/Sci-Fi genre average $194 million.
- Longer films tend to be more successful, more specifically the 130 to 140-minute range.
- - Action/Adventure/Sci-Fi films averaged 139 minutes.

## Next Steps

Further analyses could yield additional insights that may influence Microsoft’s film making decisions.
- Financial data was from 2010-2018
- - Compare this data to current (2022) trends
- - See if market is changing
- Directors/Actors
- - Determine actor and director trends
- - See if certain people do better in certain markets
- Writers
- - Research veteran and up and coming writers

## For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/rustyb08/phase_1_project/blob/main/Microsoft%20Original%20Content.ipynb) or review this [presentation](https://github.com/rustyb08/phase_1_project/blob/main/Microsoft%20Original%20Content.pdf).

