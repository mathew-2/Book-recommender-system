# Book Recommender System

Welcome to the Book Recommender System! This project is a collaborative-filtering recommendation system that suggests books based on user preferences and reading history. The system leverages user ratings and book metadata to generate personalized book recommendations.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [How it Works](#how-it-works)
- [Improvements](#improvements)
- [Contributing](#contributing)
- [License](#license)

## Overview

This book recommender system uses collaborative filtering and other techniques to suggest books that a user might enjoy. By analyzing user ratings and book metadata, the system can identify patterns and similarities to provide personalized recommendations.

## Features

- Collaborative filtering to suggest books based on user ratings.
- Utilizes book metadata such as authors, genres, and more.
- Easy-to-use interface powered by Flask.
- Displays popular books with ratings and images on the home page.

## Installation

To run this project locally, follow these steps:

1. Clone this repository:
    ```sh
    git clone https://github.com/your-username/book-recommender-system.git
    cd book-recommender-system
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

3. Ensure you have the necessary pickle files (`popular.pkl`, `books.pkl`, `pt.pkl`, and `similarity_scores.pkl`) in your project directory.

4. Run the Flask app:
    ```sh
    python app.py
    ```

## Usage

1. Open your web browser and go to `http://localhost:5000`.
2. The home page will display popular books with their ratings and images.
3. To get book recommendations:
   - Click on the "Recommend" tab.
   - Enter the name of a book you like.
   - The system will recommend similar books based on collaborative filtering.

## How it Works

1. **Data Loading**: The system loads book data from preprocessed pickle files.
2. **Data Preprocessing**: It processes the data to extract relevant information such as genres, authors, etc.
3. **Collaborative Filtering**: The system uses collaborative filtering to find similarities between users and books.
4. **Similarity Calculation**: It calculates the similarity between books using cosine similarity based on user ratings.
5. **Recommendation**: Based on the similarity scores, the system recommends books that are most relevant to the user.

### Flask App Structure

- `app.py`: The main Flask application file that defines the routes and logic for rendering templates and handling recommendations.
- `templates/index.html`: The home page template displaying popular books.
- `templates/recommend.html`: The recommendation page template where users can input their favorite books and see recommendations.

## Improvements

Here are some potential improvements to enhance the recommender system:

- **Incorporate More Features**: Including additional features like user demographics, reading habits, etc., can improve recommendations.
- **Hybrid Approach**: Combining collaborative filtering with content-based filtering to leverage both user interaction data and book metadata.
- **Optimization**: Improving the efficiency of data processing and similarity calculations.
- **User Interface**: Enhancing the Flask app interface for a better user experience.

Feel free to fork the repository and submit pull requests for any improvements or additional features.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for review.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
