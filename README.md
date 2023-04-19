# Movie-Recommendation-System-using-ML
Demographic Filtering recommender system implemented using ML









Demographic Filtering is one of the three types of recommender systems. The other two are:
- Content Based Filtering
- Collaborative Filtering

Here, we'll use demographic filtering. They offer generalized recommendations to every user, based on movie popularity and/or genre. The System recommends the same movies to users with similar demographic features. The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.<br>


For this, we need a metric to score or rate the movie, calculate the score for every movie and then, sort the score and recommend the best rated movies.


So, I'll be using IMDB's Weighted Rating :-<br>

![Picture of the IMDB Weighted Rating Formula](https://1.bp.blogspot.com/-IwW-xX59Hi4/YF7TyvzmM7I/AAAAAAAAdkg/34Mpp3aW5LAsy561icqkdDEsq_O2ZgI9gCLcBGAsYHQ/s762/weight-avg.png)

where
<ul>
    <li><strong>v</strong> is the number of votes for the movie</li>
   <li><strong>m</strong> is the minimum votes required to be listed in the chart</li>
    <li><strong>R</strong> is the average rating of the movie</li>
    <li><strong>C</strong> is the mean vote across the whole report</li>

