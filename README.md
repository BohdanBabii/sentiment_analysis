# Twitter Sentiment Analysis Project

## Overview

This project focuses on applying advanced machine learning techniques to perform sentiment analysis on Twitter data. The primary goal is to classify tweets as either positive or negative using models such as Logistic Regression, Naive Bayes, and Support Vector Machines (SVM). The project is implemented in a structured Jupyter Notebook environment, providing a comprehensive analysis of each model's performance across different dataset sizes.

## Repository Structure

- **data.csv**: Contains tweets with labels for training.
- **data_validation.csv**: Used to evaluate the model with unseen data.
- **sentiment_analysis.ipynb**: The Jupyter Notebook containing the entire implementation, from data preprocessing to model evaluation.

## Setup Instructions

### 1. Prerequisites

Ensure that you have the following software installed:
- Python 3.x
- Jupyter Notebook
- Required Python libraries as listed in the `requirements.txt` file.

### 2. Installation

1. Clone this repository to your local machine using:
    ```bash
    git clone https://github.com/BohdanBabii/sentiment_analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd sentiment_analysis
    ```
3. Install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2. Open `sentiment_analysis.ipynb` in the Jupyter interface.
3. Run the cells sequentially to execute the full analysis, from data preprocessing to model evaluation.

## Project Details

### Data Preprocessing

- **Cleaning**: The tweets are cleaned by removing URLs, mentions, hashtags, numbers, and special characters. All text is converted to lowercase for consistency.
- **Transformation**: Different transformation methods are used depending on the model. For Logistic Regression, TF-IDF vectorization is applied, while Naive Bayes and SVM use CountVectorizer.

### Models

- **Logistic Regression**: A statistical method used for binary classification. The model was trained with TF-IDF features.
- **Naive Bayes**: A probabilistic classifier based on Bayes' theorem with strong independence assumptions. The model was trained with CountVectorizer features.
- **Support Vector Machine (SVM)**: A robust classifier well-suited for high-dimensional spaces. The model was trained with CountVectorizer features.

### Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **Training Time**

## Results

- Logistic Regression showed the best performance, especially when trained on the full dataset of 500,000 tweets, achieving an accuracy of 81.875%.
- Naive Bayes and SVM also performed well, with SVM showing higher computational demands as dataset size increased.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

