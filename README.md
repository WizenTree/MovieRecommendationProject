# Movie Recommendation System

## Project Summary

This project builds a movie recommendation system using various movie attributes. The system leverages keywords, genres, overviews, titles, spoken languages, and production countries to find similar movies. It employs text processing techniques and similarity metrics to provide recommendations based on a given movie title.

## Tech Stack

*   **Python:** The core programming language for the project.
*   **pandas:** Used for data manipulation and analysis.
*   **numpy:** Used for numerical operations.
*   **scikit-learn:** Provides tools for text feature extraction (`TfidfVectorizer`, `CountVectorizer`) and similarity calculation (`cosine_similarity`).
*   **nltk:** Used for natural language processing tasks such as removing stopwords and lemmatization.
*   **ast:** Used for safely evaluating string literals.
*   **fuzzywuzzy:** Used for fuzzy string matching to handle potential typos in movie titles.
*   **gdown:** Used for downloading the dataset from a Google Drive link.

## Key Learnings and Findings

*   Combining multiple features (overview, keywords, genres, countries, languages) significantly improves the quality of movie recommendations compared to using a single feature.
*   Text processing techniques like stopword removal and lemmatization are crucial for standardizing textual data before calculating similarity.
*   Different vectorization methods (TF-IDF for overviews, CountVectorizer for keywords) can be used effectively for different types of textual data.
*   Using a combination of cosine similarity (for vector spaces) and Jaccard similarity (for set-like data) provides a comprehensive measure of movie similarity.
*   Implementing fuzzy matching for movie titles helps in handling user input errors and improving the robustness of the recommendation system.
*   Weighting different similarity measures allows for fine-tuning the recommendation process based on the importance of each feature.

## Project Structure

The notebook is organized into the following sections:

1.  **Importing Libraries:** Imports all necessary Python libraries.
2.  **Downloading the Dataset:** Downloads the movie dataset.
3.  **Loading and Exploring the Data:** Loads the data into a pandas DataFrame and performs initial exploration.
4.  **Handling Missing Values:** Addresses missing values in the dataset.
5.  **Handling Duplicate Rows:** Removes duplicate entries.
6.  **Downloading NLTK Resources:** Downloads required NLTK data.
7.  **Defining Text Cleaning Functions:** Defines functions for text preprocessing.
8.  **Defining Jaccard Similarity:** Defines a function to calculate Jaccard similarity.
9.  **Processing List-like Features:** Converts string representations of lists into actual Python lists.
10. **Cleaning and Preparing Features:** Cleans and standardizes the features for similarity calculation.
11. **Feature Extraction and Similarity Calculation:** Applies vectorization and calculates similarity matrices.
12. **Extracting Movie Information:** Extracts lists of movie attributes.
13. **Defining Combined Similarity Function:** Defines a function for calculating combined similarity scores.
14. **Getting Movie Recommendations:** Defines the main function for generating recommendations.
15. **Getting Recommendations for "Terminator":** Demonstrates how to use the recommendation function.

## How to Run

1.  Open the notebook in Google Colab or a Jupyter Notebook environment.
2.  Ensure you have the necessary libraries installed (or run the cells that install them).
3.  Run the cells sequentially from top to bottom.
4.  Modify the last cell to get recommendations for a different movie title.

## Dataset

The dataset used in this project is downloaded from a Google Drive link provided within the notebook. It contains various movie attributes.
The dataset is originally from Kaggle. I have used Google Drive for easier access in Google Colab, because uploading large files manually takes a lot of time in Google Colab. 

