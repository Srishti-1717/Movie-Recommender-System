# Movie Recommender System

This project is a machine learning-based movie recommender system that provides movie recommendations based on various features such as genres, cast, crew, and keywords. The system uses the **5000 Movies Dataset** and **Credits Dataset** from Kaggle to train the recommendation model, and it is deployed using **Heroku**.

## Datasets

The system utilizes two main datasets from Kaggle:
1. **Movies Dataset**: Contains information about 5000 movies, including titles, genres, overviews, and release dates.
2. **Credits Dataset**: Contains detailed information about the cast and crew of each movie.

These datasets were preprocessed and transformed to extract important features used for recommending similar movies based on user input.

## Machine Learning Techniques

### 1. Feature Engineering
- The movie titles, genres, keywords, and crew information from the datasets were tokenized and vectorized using **TF-IDF** (Term Frequency-Inverse Document Frequency) to convert textual data into numerical representations.
- The feature vectors were then used to measure the similarity between movies.

### 2. Cosine Similarity
- After vectorizing the relevant features, **cosine similarity** was applied to compute the similarity scores between movies.
- Based on a given movie, the model suggests similar movies by comparing their cosine similarity scores.

### 3. TMDB API Integration
- The system is integrated with the **TMDB API** to retrieve additional movie details such as posters, ratings, and overviews to enhance the user experience.

## Model Deployment

The final model was deployed on **Heroku** using PyCharm. Pycharm serves the recommendation model by providing it a web interface and interacts with the TMDB API to provide movie recommendations to users. The deployment process involved:
- Importing and installing certain libraries and adding files to the Pycharm application.
- Deploying the system on Heroku for public access.

## Technologies Used

- **Python**: For data manipulation and building the recommendation model.
- **Pandas & NumPy**: For handling and transforming datasets.
- **scikit-learn**: For vectorization and similarity computation.
- **Pychar,**: For building the web interface.
- **Heroku**: For deployment.
- **TMDB API**: For fetching additional movie information.

---

This project demonstrates how machine learning techniques can be applied to build a personalized recommendation system by leveraging movie datasets, transforming features, and deploying the model on a scalable platform like Heroku.
