# EECS_731_MS_Project_3
  Blockbuster or art film?
1. Set up a data science project structure in a new git repository in your GitHub account
2. Download the one of the MovieLens datasets from https://grouplens.org/datasets/movielens/
3. Load the data set into panda data frames
4. Formulate one or two ideas on how the combination of ratings and tags by users helps the data set to establish additional value using exploratory data analysis
5. Build one or more clustering models to determine similar movies to recommend using the other ratings and tags of movies by other users as features
6. Document your process and results
7. Commit your notebook, source code, visualizations and other supporting files to the git repository in GitHub

In this project I used the above instruction to create a movie recommendation code where movie titles are used as inputs and the ten most similar movies are given as an output. I used the small dataset due to limited computational space and found that both Kmeans and Agglomerative Clustering did a good job in recommending movies similar to the suggested one. 
Some of the feature engineering required to get menaingful data from reviews included using a Baysien weighted average. This allowed for highly reviewed movies to have a more meaningful rating than titles that were reviewed less. 
The use of K means to determine the distance between data points and a centroid and that groups together the points up to a certain distance away. This worked suprisingly well espesially with how simple the method was.
The next method used to determine potential movies to watch was Agglomerative Clustering. This is a hierarchical clustering technique that starts from a bottom up approach and pairs clusters together as it moves up the hierachy. We also set the same number of clusters for the method to find. It begins comnbining clusters to minimize a linkage distance until the number of clusters reaches the set number. This worked nearly the same as the K means but I think that if there are more clusters to be found that starting with this method would give you a smaller more related cluster than k means would. 
Overall this project gave a great example of how to engineer features to give them meaning as well as how to use those features to cluster related data.
