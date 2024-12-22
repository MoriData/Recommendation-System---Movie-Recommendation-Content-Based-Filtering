# Movie Recommendation System: Content-Based Filtering

This repository contains a project that implements a content-based movie recommendation system. The recommendation system uses cosine similarity to recommend movies based on their overviews and keywords. The system is built using the TMDb Movies Dataset.

## Project Overview
The project aims to provide personalized movie recommendations by analyzing movie metadata. It uses natural language processing and cosine similarity to find the closest matches to a user's input.

### Key Features:
- Content-based filtering using movie overviews and keywords.
- Efficient similarity computations for large datasets.
- Interactive Jupyter Notebook implementation.

## Dataset
The dataset used for this project is the **TMDb Movies Dataset 2023** from [Kaggle](https://www.kaggle.com/datasets/). The dataset contains metadata for approximately 930,000 movies. For efficient processing, the project limits the dataset to the first 25,000 rows.

### Preprocessing Steps:
1. Extracted movie overviews and keywords.
2. Converted text data into vectors using TF-IDF (Term Frequency-Inverse Document Frequency).
3. Calculated cosine similarity scores between movies.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/MoriData/Recommendation-System---Movie-Recommendation-Content-Based-Filtering.git
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook recommendation-system-movie-recommendation.ipynb
   ```
2. Follow the step-by-step instructions in the notebook to:
   - Preprocess the dataset.
   - Build the recommendation system.
   - Test with sample movie titles.

## Project Structure
- `recommendation-system-movie-recommendation.ipynb`: The main notebook containing the implementation.
- `requirements.txt`: List of required Python libraries.
- `README.md`: Project documentation (this file).

## How It Works
1. **Data Preprocessing**:
   - Text data (overviews and keywords) is cleaned and transformed into a TF-IDF matrix.
   - This matrix captures the importance of terms within the dataset.
2. **Cosine Similarity**:
   - Cosine similarity is calculated between movies based on their TF-IDF vectors.
   - Movies with higher similarity scores are recommended.
3. **User Interaction**:
   - Input a movie title to get a list of recommended movies.

## Limitations
- Recommendations are limited to the data available in the dataset.
- The system doesn't account for user preferences beyond movie metadata.
- Performance is constrained by the size of the processed dataset.

## Future Enhancements
- Expand the dataset to include more movies.
- Incorporate additional features such as genres, cast, and ratings.
- Implement collaborative filtering to complement content-based recommendations.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- The dataset is provided by [Kaggle](https://www.kaggle.com/).
- Cosine similarity and TF-IDF methods are fundamental concepts in text analysis and information retrieval.

---

Feel free to contribute to this project by submitting issues or pull requests!
