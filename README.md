# Movie-Recommendation-System

#### Created and Tested with Python 3.9

#### A web app that recommends you movies based on the movie you search as well as all the details of the movie along with its trailer and reviews.

## Getting started

#### In order to start with the Movie Recommendation System, just clone this repository and download the TMDB movie dataset from kaggle from the below given link.

#### https://www.kaggle.com/datasets/ahsanaseer/top-rated-tmdb-movies-10k

#### Now create a virtual environment with Python 3.9 and then install the packages in the requirements.txt file.

#### Run the Main.ipynb file in your system and it will generate 2 files: movie_list.pkl and similarity.pkl, Now you just need to open your front end part by extracting the frontend.zip and open VS Code and just run the command streamlit run app.py
<img width="1440" alt="Movie Recommendation System Screenshot" src="https://github.com/anu24765/Movie-Recommendation-System/assets/96810206/b7f0a545-3672-4c5c-9a78-4b2268d74ea5">



## How to get the API key?

#### Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your API sidebar once your request is approved.
## How it works?

#### 1. The system reads a dataset containing movie information (`dataset.csv`) using pandas.

#### 2. Feature selection is performed to select relevant features for recommendation. The selected features include 'id', 'title', 'overview', and 'genre'.

#### 3. A new feature 'tags' is created by concatenating 'overview' and 'genre' to represent each movie.

#### 4. The CountVectorizer from scikit-learn is used to convert text data into a numerical format suitable for machine learning.

#### 5. Cosine similarity is computed between the feature vectors of movies to measure their similarity.

#### 6. The system provides a function `recommend(movies)` that takes a movie title as input and returns the top 5 recommended movies based on content similarity.

#### 7. The recommended movies are printed to the console.

#### 8. The system saves the processed data and similarity matrix using pickle for future use.

#### The web app has been created using streamlit.

## Contribution

#### Once you get a better understanding of the project, you will see that a lot can be done with the project. You can work with improving the recommendation or add more of the latest movie data from different sites and work on them as well. You can also improve the interface by either adding more features in the web app or using other better web based applications like Django and Flask and many more. Pull requests for any changes are accepted. Feel free to fork this project and make your own changes too.
