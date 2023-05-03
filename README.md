<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
    <h1>Simple Movie Recommendation System using KNN</h1>
    <p>This Jupyter Notebook demonstrates a simple movie recommendation system using the K-Nearest Neighbors algorithm. The dataset used in this project contains information about movies and their ratings, which will be used to predict similar movies that a user might be interested in watching.</p>
css
Copy code
<h2>Importing Required Libraries and Dataset</h2>
<p>The necessary libraries such as Pandas, NumPy, Matplotlib, Seaborn and warnings are imported in the first few lines of code. Two datasets, namely 'movies.txt' and 'rating.txt', are imported using the Pandas library.</p>

<h2>Data Cleaning and Preparation</h2>
<p>The two datasets are merged based on the 'movieId' column, and unnecessary columns such as 'timestamp' and 'genres' are dropped. The resulting dataframe is then checked for any null values.</p>

<h2>Filtering Popular Movies</h2>
<p>A popularity threshold is set to 50, and movies with a total rating count greater than or equal to this threshold are selected. This helps filter out less popular and less rated movies from the dataset.</p>

<h2>Creating a Pivot Table and Applying KNN Algorithm</h2>
<p>The selected movies are then used to create a pivot table where each row represents a movie and each column represents a user. The pivot table is then converted to a sparse matrix, and KNN algorithm is applied on this matrix. This algorithm helps identify similar movies based on their rating patterns.</p>

<h2>Displaying Recommendations</h2>
<p>A random movie is selected from the pivot table, and the KNN algorithm is used to identify 5 movies that are similar to this movie. The selected movie and its related movies are then displayed on the output screen.</p>
  </body>
</html>
