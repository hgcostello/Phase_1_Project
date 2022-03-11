# Analyis of Movie Data

By: Henry Graham Costello

## Summary

This project takes data from three major sources:
1. IMDB
2. Box Office Mojo
3. The Movie Database

IMDB Data has basic information on over 100,000 movies -- information like Title, Year, Genre, Runtime, etc. IMDB also has information on the fan rating of a subset (73,000) of these movies.

Box Office Mojo contains data on the domestic and foreign success of just over 3,000 films.

The Movie Database contains more detailed 'basic' information -- namely Release Date for our purposes -- on over 25,000 movies.

As you can imagine, there is a large degree of overlap between the two large IMDB datasets. We are interested in examining financial success, which means that our common denominator is ultimately Box Office Mojo, the smallest data set of the group. This is cutting at minimum about 3/4 of the data contained in the other three data sets. This is an important selection bias to be aware of.

We will illustrate relationships between several variables and Gross Success: Fan Rating, Genre, and Season of Release.

# Results
### It doesn't seem to matter whether or not the fans like your movie.
As we can see from the graph below, there does not appear to be a strong link between movie rating and gross success.
This visual suggestion is confirmed by a low correlation: ~ 0.026

![download](https://user-images.githubusercontent.com/91205382/157929587-7d3dbb95-97cd-4d10-bf1c-375677d16f06.png)

Another interesting takeaway from this graph is the fact that most movie are clustered in low gross success range.
There are very few billion dollar plus movies and those datapoints are dragging the y-axis up.


### What are the most successful genres? Sci-Fi, Animation, Adventure, Action, Fantasy
For this graph, we cut the top 2% of values for gross success. More explicitly, we took the 98th percentile of gross success and set every value greater than that to the value at the 98th percentile. This will lower the bounds of the y-axis.
Below, you can see a boxplot displaying median, IQR, max/min of total gross by the genre of film.

![download-1](https://user-images.githubusercontent.com/91205382/157931294-a0012b11-ffaf-4026-bc24-1f835d642e22.png)

As we can see, the most successful film genres appear to be, in order, Sci-Fi, Animation, Adventure, Action, Fantasy.

### Lastly we examime commercial success by season of release
Below you will find a boxplot displaying key diagnostics of success for movies released in the Summer, Spring, Fall and Winter.
For this graph, we cut the top 10% of values for gross success using same methodology as the graph above.

![download-2](https://user-images.githubusercontent.com/91205382/157932128-e9056616-0c8a-441f-a6bd-d93115e376f4.png)

## Conclusions

Although our data is limited, three key suggestions arise from the findings:
1. Don't be overly concerned about how much the fans 'like' the film. Whether this is because the quality truly doesn't matter, or polarizing movies are more successful than cult classics, the data indicates that there is very low correlation, if any, between fan rating and gross success.

## Next Steps

Narrowing down our parameters. We can provide more conclusive recommendations if Microsoft has some preliminary thoughts about what type of studio they want to run and what type of movies they want to make.

