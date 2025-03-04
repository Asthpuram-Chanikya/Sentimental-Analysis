# Movie Review Sentiment Analysis

A natural language processing model that classifies movie reviews as positive or negative using the NLTK movie_reviews dataset and scikit-learn's Naive Bayes classifier.

## Project Overview

This project implements a simple yet effective sentiment analysis system that:
- Processes text data from movie reviews
- Converts text into numerical features using bag-of-words approach
- Trains a Multinomial Naive Bayes classifier
- Provides a prediction function for analyzing new review texts

## Features

- **Data Processing**: Transforms raw movie review text into structured data
- **Text Vectorization**: Converts text to numerical features using CountVectorizer
- **Machine Learning Model**: Implements a Naive Bayes classifier for sentiment prediction
- **Performance Metrics**: Evaluates model using accuracy, precision, recall, and F1-score
- **User Interface**: Simple command-line interface for entering new reviews to analyze

## Technologies Used

- Python 3.x
- NLTK (Natural Language Toolkit)
- scikit-learn
- pandas

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/movie-sentiment-analysis.git
   cd movie-sentiment-analysis
   ```

2. Install the required dependencies:
   ```
   pip install nltk pandas scikit-learn
   ```

3. Download the necessary NLTK data:
   ```python
   import nltk
   nltk.download('movie_reviews')
   ```

## Usage

Run the script to train the model and start predicting:

```
python sentiment_analyzer.py
```

When prompted, enter a movie review text, and the model will classify it as either 'pos' (positive) or 'neg' (negative).

### Example

```
Input: "The plot was captivating and the acting was phenomenal. Highly recommended!"
Output: pos

Input: "Boring storyline with terrible dialogue and wooden performances."
Output: neg
```

## Model Performance

The Multinomial Naive Bayes model achieves approximately 80-85% accuracy on the test set, with balanced precision and recall metrics for both positive and negative classes.

## Project Structure

```
movie-sentiment-analysis/
├── sentiment_analyzer.py    # Main script with model implementation
├── README.md                # Project documentation
└── requirements.txt         # Required dependencies
```

## Future Improvements

- Implement more advanced NLP techniques like word embeddings or BERT
- Create a web interface for easier interaction
- Add support for multi-class sentiment analysis (e.g., very negative, negative, neutral, positive, very positive)
- Expand the training dataset to improve model robustness

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- NLTK for providing the movie_reviews corpus
- scikit-learn for the machine learning tools
- The open-source community for continuous inspiration and support

[Creating Great README Files for Your Python Projects](https://realpython.com/readme-python-project/) 
