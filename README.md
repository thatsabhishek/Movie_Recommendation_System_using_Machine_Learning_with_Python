# Movie Recommendation System using Machine Learning with Python

## Overview
This project implements a movie recommendation system using machine learning techniques in Python. The system recommends movies based on their similarity to a user's favorite movie. The code utilizes the scikit-learn library for text vectorization and cosine similarity calculations.

## Code Structure
The code is organized into the following sections:

1. **Data Loading:**
   - The movie data is loaded from a CSV file (`movies.csv`) using pandas.
   - The first 5 rows of the dataset and its dimensions are printed for initial exploration.

2. **Feature Selection:**
   - Relevant features for recommendation, including 'genres', 'keywords', 'tagline', 'cast', and 'director', are selected.
   - Null values in these features are replaced with empty strings.

3. **Text Vectorization:**
   - The selected features are combined into a single text feature.
   - TF-IDF vectorization is applied to convert the text data into feature vectors.

4. **Cosine Similarity:**
   - Cosine similarity scores between movies are calculated based on their feature vectors.

5. **User Input:**
   - The user is prompted to input their favorite movie.

6. **Movie Recommendation:**
   - A list of movie titles from the dataset is created.
   - Using difflib, the closest match to the user's input is found.
   - The index of the matched movie is used to retrieve similarity scores with other movies.
   - The movies are sorted based on their similarity scores, and the top suggestions are presented to the user.

## How to Use
1. **Clone the Repository:**
   ```
   git clone https://github.com/your-username/Movie_Recommendation_System_using_Machine_Learning_with_Python.git
   cd Movie_Recommendation_System_using_Machine_Learning_with_Python
   ```

2. **Install Dependencies:**
   ```
   pip install pandas numpy scikit-learn
   ```

3. **Run the Code:**
   - Ensure that the `movies.csv` file is present in the same directory.
   ```
   python movie_recommendation_system.py
   ```

4. **Enter Favorite Movie:**
   - Follow the prompts to enter the name of your favorite movie.

5. **Review Recommendations:**
   - The code will display a list of movie recommendations based on the input.
