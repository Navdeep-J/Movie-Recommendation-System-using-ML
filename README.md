# Movie-Recommendation-System-using-ML
Demographic Filtering recommender system implemented using ML<hr>

The created recommendation system will be a Demographic Filtering recommender system.

## Dataset
I've used the <a href ="https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata">TMDB 5000 Movie Dataset</a>. This contains 2 datasets.  <br>

The first dataset contains the following features:-

- movie_id - A unique identifier for each movie.
- cast - The name of lead and supporting actors.
- crew - The name of Director, Editor, Composer, Writer etc.


The second dataset has the following features:-

- budget - The budget in which the movie was made.
- genre - The genre of the movie, Action, Comedy ,Thriller etc.
- homepage - A link to the homepage of the movie.
- id - This is infact the movie_id as in the first dataset.
- keywords - The keywords or tags related to the movie.
- original_language - The language in which the movie was made.
- original_title - The title of the movie before translation or adaptation.
- overview - A brief description of the movie.
- popularity - A numeric quantity specifying the movie popularity.
- production_companies - The production house of the movie.
- production_countries - The country in which it was produced.
- release_date - The date on which it was released.
- revenue - The worldwide revenue generated by the movie.
- runtime - The running time of the movie in minutes.
- status - "Released" or "Rumored".
- tagline - Movie's tagline.
- title - Title of the movie.
- vote_average - average ratings the movie recieved.
- vote_count - the count of votes recieved.


## Demographic Filtering
Demographic Filtering is one of the three types of recommender systems. The other two are:
- Content-Based Filtering
- Collaborative Filtering

Here, I'll use demographic filtering. Such recommender systems offer generalized recommendations to every user, based on movie popularity and/or genre. The System recommends the same movies to users with similar demographic features. The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.<br>


For this, we need a metric to score or rate the movie, calculate the score for every movie, and then, sort the score and recommend the best-rated movies.


So, I'll be using IMDB's Weighted Rating:-<br>

![Picture of the IMDB Weighted Rating Formula](https://1.bp.blogspot.com/-IwW-xX59Hi4/YF7TyvzmM7I/AAAAAAAAdkg/34Mpp3aW5LAsy561icqkdDEsq_O2ZgI9gCLcBGAsYHQ/s762/weight-avg.png)

where
<ul>
    <li><strong>v</strong> is the number of votes for the movie</li>
   <li><strong>m</strong> is the minimum votes required to be listed in the chart</li>
    <li><strong>R</strong> is the average rating of the movie</li>
    <li><strong>C</strong> is the mean vote across the whole report</li>
    </ul>
    
    
After finding the Weighted Rating (calc_score), we'll sort the list and print 10 movies with the highest ratings. then, we'll find the 10 most popular movies.
    
    
## Concepts used
    - pandas library
    - numpy library
    - matplotlib library
    - Machine learning concepts
    - Recommender systems
    
    
