# Movie Recommendation System

This project is a content-based movie recommendation system built using Python. It leverages movie metadata to recommend similar movies based on user input. The system uses natural language processing (NLP) techniques and cosine similarity to compute recommendations.

## Features

- **Content-Based Recommendations**: Recommends movies based on their metadata, such as genres, keywords, cast, and crew.
- **Data Preprocessing**: Cleans and processes movie data for analysis.
- **Vectorization**: Converts textual data into numerical vectors using `CountVectorizer`.
- **Similarity Calculation**: Computes cosine similarity between movies to find the most similar ones.
- **Interactive Recommendations**: Allows users to input a movie title and get a list of similar movies.

## Dataset

The project uses the following datasets:
- `tmdb_5000_movies.csv`: Contains metadata about movies.
- `tmdb_5000_credits.csv`: Contains information about the cast and crew of movies.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
   cd movie-recommendation-system

2. Install the required Python packages:

3. Download the datasets (tmdb_5000_movies.csv and tmdb_5000_credits.csv) and place them in the project directory.

Usage
1. Run the Jupyter Notebook mrs.ipynb to preprocess the data and build the recommendation system.

2. Use the recommend function to get movie recommendations:
   recommend('Top Gun')

4. Save the processed data and similarity matrix for future use:
   pickle.dump(new_df.to_dict(), open('movie_dict.pkl', 'wb'))
   pickle.dump(similarity, open('similarity.pkl', 'wb'))

Project Structure
.
├── [app.py](http://_vscodecontentref_/0)                  # (Optional) Flask app for deploying the recommendation system
├── [mrs.ipynb](http://_vscodecontentref_/1)               # Jupyter Notebook containing the implementation
├── [tmdb_5000_movies.csv](http://_vscodecontentref_/2)    # Movie metadata
├── [tmdb_5000_credits.csv](http://_vscodecontentref_/3)   # Cast and crew data
├── [movie_dict.pkl](http://_vscodecontentref_/4)          # Pickled movie metadata dictionary
├── [similarity.pkl](http://_vscodecontentref_/5)          # Pickled similarity matrix
├── requirements.txt        # Python dependencies

Key Libraries Used
• Pandas: For data manipulation and preprocessing.
• NumPy: For numerical operations.
• NLTK: For stemming and text preprocessing.
• Scikit-learn: For vectorization and similarity computation.
• Pickle: For saving and loading processed data.

Example Output
Input:
recommend('Top Gun')

Output:
A Guy Named Joe
Pearl Harbor
Highway
Broken Arrow
Firefox

Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
The datasets are sourced from The Movie Database (TMDb).
Special thanks to the open-source community for providing the tools and libraries used in this project.
