ABOUT:

All of us love to watch movies! There is a disliking for some of the movies and liking at the same point.  Many people prefer a specificgenre of films. In today’s 
world with the power of Machine Learning and its algorithms we can predict a similarity among various movies which can serve as a great application in Movie 
Recommender Systems. We can categorize the films on their plot similarities just by mere institution which is no fun in Data Science context. In this paper we are 
trying to find the resemblance in the movies on the basis of their content available on IMDb and Wikipedia. First the data is preprocessed using tokenization,
Stemming etc. and converted into plain text. The model is trained using TF-IDF Vectorizer. Then the similarity among the movies is calculated using Similarity 
Metrics. On the basis of similarity, we assign the movies into different subgroups using clustering technique, an Unsupervised Machine Learning approach. We then 
try to visualize the proximity of the movies using a hierarchical structure. Finally, we evaluate the best ‘k’ for our clustering analysis and evaluate it using 
the elbow test.

DATASET:

We are taking the movie synopsis of each movie from Wikipedia and IMDb simultaneously for about 100 English movies. The plots are directly extracted from Wikipedia 
and IMDb using the python Wikipedia API by installing the Wikipedia package and the IMDb package. The plots extracted from Wikipedia and IMDb for each movie convey 
the same story but they vary in the style of writing and linguistic expression. They also differ in terms of their features for example one feature may be 
elaborated in one plot but not in other. The data is imported in a comma separated format. The dataset contains the following features with their description as 
follows:

 rank: This is used for ordering the
movies from 0 to 99.

 title: This column contains the name
description of the particular movie.

 genre: This contains the type of movie.

 wiki_plot: This contains the Wikipedia

plot.

 imdb_plot: This contains the IMDb
plot.
