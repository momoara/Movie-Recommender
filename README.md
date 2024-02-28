# Movie Recommendation System

This project implements a movie recommendation system using the TMDB 5000 Movie Dataset. The system uses a content-based filtering approach, leveraging movie metadata such as genres, keywords, main actors, and director to recommend movies similar to a given movie.

## Overview

The recommendation system is built on Python, utilizing libraries such as Pandas, NumPy, and Scikit-learn. The core algorithm is based on calculating the cosine similarity between movies using their metadata features, allowing for personalized movie recommendations.

## Features

- **Data Preprocessing**: Cleans and prepares the TMDB movie dataset for analysis.
- **Feature Engineering**: Extracts and combines relevant features such as genres, keywords, main actors, and director from the movie metadata.
- **Recommendation Algorithm**: Utilizes TF-IDF vectorization and cosine similarity to find movies that are most similar to a given input movie.

## Setup and Installation

Ensure you have Python installed on your system. The project requires the following Python libraries:

- Pandas
- NumPy
- Scikit-learn

You can install these libraries using pip:

```bash
pip install pandas numpy scikit-learn
```

## Usage

To use the recommendation system, run the Python script and enter the title of the movie you like. The system will then display a list of recommended movies based on the input.

Example:

```python
print(get_recommendations('The Matrix'))
```

## Data

The TMDB 5000 Movie Dataset is utilized in this project, containing metadata on over 5,000 movies. The dataset includes two files: `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`, which are merged and processed to extract relevant features for the recommendation system.

## Methodology

The project follows these key steps:

1. **Data Exploration and Preprocessing**: Understands the structure of the data, cleans, and prepares it for modeling.
2. **Feature Engineering**: Identifies and combines relevant features from the dataset.
3. **Model Development**: Builds the recommendation model using TF-IDF vectorization and cosine similarity.
4. **Evaluation**: Tests the model to assess its performance in recommending similar movies.

## Limitations and Future Work

The current implementation is a basic version of a content-based recommendation system. Future enhancements can include:

- Incorporating user ratings and reviews for a more personalized recommendation.
- Exploring more sophisticated algorithms like collaborative filtering and hybrid models.
- Implementing a more interactive user interface for easier navigation and usage.

## Contributing

Contributions to improve the recommendation system are welcome. Please feel free to fork the repository, make changes, and submit a pull request.

## License

This project is open-sourced under the MIT License. See the LICENSE file for more details.
