# Book Recommendation System

A machine learning-based book recommendation system that suggests personalized book recommendations based on user preferences, ratings, or book attributes.

## Features
- **Personalized Recommendations**: Suggests books tailored to user input or historical data.
- **Collaborative Filtering**: Recommends books based on user ratings and similarities (if applicable).
- **Content-Based Filtering**: Suggests books based on genres, authors, or descriptions (if applicable).
- **Simple Interface**: Provides an easy-to-use command-line or web interface for exploring recommendations.
- **Scalable**: Designed to handle large datasets of books and users.

## Methodology

- **Data Loading**: Import and clean data from CSV files
- **Feature Engineering**: Extract tag-based features using TF-IDF
- **Similarity Calculation**: Compute cosine similarity between books
- **Recommendation**: Suggest top N similar books based on the selected title

## Dataset
This project uses the GoodBooks-10k dataset from Kaggle, which contains ratings for 10,000 books with 6 million ratings from 53,000 users, along with book metadata and tags for recommendation purposes.
- **Source**: https://www.kaggle.com/zygmuntz/goodbooks-10k

## Technologies Used
Python: Core programming language.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computations.
- **Surprise**: For collaborative filtering using the SVD algorithm.
- **Scikit-learn**: For content-based filtering with TF-IDF and cosine similarity.
- **Jupyter Notebook**: For the interactive development environment.
- **IPyWidgets**: For interactive user inputs in the notebook.
- **Dataset**: GoodBooks-10k from Kaggle.

## Installation
To set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/anamikapati/book-recommendation.git
   cd book-recommendation
2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
3. **Install Dependencies**:
   Ensure you have Python 3.8+ installed. Then, install required packages:
   ```bash
   pip install -r requirements.txt

## Results

Here is a sample output of the recommendation system:

**Input**: "The Hobbit"

**Top 5 Recommended Books**:
1. The Fellowship of the Ring
2. The Return of the King
3. The Two Towers
4. A Game of Thrones
5. The Chronicles of Narnia

These results are generated using TF-IDF vectorization of tag metadata followed by cosine similarity computation. The system finds books with high textual similarity in tags to the selected title.

## Contact
- Author: Anamika Pati
- Email: anamika24300@iiitnr.edu.in
- GitHub: [anamikapati](https://github.com/anamikapati)

## Acknowledgements

- [Goodbooks-10K Dataset](https://www.kaggle.com/zygmuntz/goodbooks-10k) – for providing a rich dataset of book metadata and user ratings.
- [scikit-learn](https://scikit-learn.org/) – for tools such as TF-IDF vectorizer and cosine similarity functions.
- The open-source Python community and forums like Stack Overflow for continuous support and learning.
