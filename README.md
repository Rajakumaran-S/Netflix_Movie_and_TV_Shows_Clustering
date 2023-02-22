# Netflix_Movie_and_TV_Shows_Clustering
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

In this project, we worked on a text clustering problem where we had to classify/group the Netflix movie/shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

- The dataset contained about 7787 records, and 11 attributes. 

- We began by dealing with the dataset's missing values and doing exploratory data analysis (EDA).

- Creating cluster using following attributes: director, cast, country, genre and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

- We used Principal Component Analysis (PCA) to handle the curse of dimensionality.

- We built Two types of clusters using the K-Means Clustering and Agglomerative Heirachycal clustering algorithm and find out optimal number of clusters using diffrent technique such as elbow method, silhoutte score and dendogram etc.

- A content based recommender system was built using the similarity matrix obtained after using cosine similarity. This recommender system will make 10 recommendations to the user based on the type of show they watched.

## Conclusion
In this project, we worked on a clustering problem wherein we had classify/group the Netflix movies and shows into certain clusters such that the shows within a cluster are similar to each other.

**Imp Insights from EDA:**


1. Movies and TV Shows on Netflix are in ratio apprx 7/3. And TV Shows have long way to catch upto the number of Movies.
2. Documentaries are the top most genre in the netflix movies. Kids TV is the top most genre in netflix TV shows.
3. Most of the movies were found to be released in the month of october, november, december and january.
4. Most content on Netflix is from United States followed by India and United Kingdom. 
5. There is a decrease in the number of shows added in the year 2020, which might be attributed to the covid-19-induced lockdowns, which halted the creation of shows.
6. Most of the movies have duration of 90 mins.
7. In the year 2019 more number of movies were released as compared to TV shows.
8. Most content o Netflix is rated for mature audience only.
9. United States and United Kingdom are closely alighned with their netflix target ages. 
* Maximum adult content is from Spain.
* Maximum teen content is from India.
* Maximum older kids content is from Japan.
* Maximum kids content is from Canada.
10. From October to January, maximum number of movies and TV shows were added on the platform.

**Clustering process:**
* Initially we have  decided to cluster the data on the basis of some  attributes like: director, cast, country, genre and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

* Through TFIDF Vectorization, we created a total of 10000 attributes.We used Principal Component Analysis (PCA) to handle the curse of dimensionality. 3500 components were able to capture more than 80% of variance, and hence, the number of components were restricted to 2600.

*  We first built clusters using the K-Means Clustering algorithm, and using elbow method and silhouette score analysis the optimal number of clusters came out to be 6.

*  Then clusters were built using the Hierarchical clustering algorithm, and the optimal number of clusters came out to be 6. This was obtained after visualizing the dendrogram.

*  A content based recommender system was built using the similarity matrix obtained after using cosine similarity. This recommender system will make 10 recommendations to the user based on the type of show they watched or searched.
