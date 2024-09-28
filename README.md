# Project Title

Analyzing Average Sentiment of Amazon Book Reviews


## Description

We conducted sentiment analysis to determine if Amazon book reviews have a positive average sentiment across categories. To drive more impactful results, we expanded our scope to identify predictive factors behind a user’s review. By using a tree-based model like random forest or decision tree, we aimed to find the most significant variables influencing reviews for future authors.
## Section 1: Software and platform

### Types of software used for the project

* Packages that should be installed in Python:
  * Numpy
  * Pandas
  * Scikit-learn
  * Matplotlib
  * Seaborn
  * Wordcloud
  * VaderSentiment
  
* Platform: Windows 10, MacOS

## Section 2: A Map of our repository

* Files (Outline)
  * DATA - Folder
    * DataAppendix.pdf
    * data.md
  * SCRIPTS - Folder
    * modeling.ipynb
    * preprocessing.ipynb
  * OUTPUT - Folder
    * IN PROGRESS 
  * LICENSE.md
  * README.md

## Section 3: Instructions for reproducing our results

* preprocessing.ipynb
  * Import software packages (os, numpy, seaborn, matplotlib, sklearn, and pandas) into python notebook
  * Define and load book_data.csv and Books_rating.csv and return both csv datasets
  * Determine each dataset's categories with '.info()' and use it for the project
  * Use '.head' method for both books and reviews datasets to return the first few rows of each dataset
  * Preprocessing (Clear missing values)
    * Rename columns and drops NaNs from important variables
    * Split helpfulness column for better understand
  * VADER Sentiment Score Assignment
    * Install '!pip install vaderSentiment' 
    * Create features (e.g. text_word_count and summary_word_count) for analysis purposes if needed
    * Save cleaned data
  
* modeling.ipynb
  * Download cleaned version of books_data and reviews_data (known as books_cleaned.csv and reviews_cleaned.csv) resulting from the preprocessing steps
  * Define and load both datasets in python
  * Establish the categories for the respective datasets with '.info()'
  * Import train_test_split and DecisionTreeRegressor to split the dataset and perform tests
  * Prepare the features (X) and target (y)
  * Create a DataFrame to show feature importance 
  * Evaluate accuracy of the model and calculate accuracy with a 10% tolerance
  * Generate additional metrics, such as mean absolute error and variance
 
* sentiment_analysis.ipynb
  * Merge the books and reviews cleaned datasets on key 'book_title', so that each review observation contains all associated book data
  * Statistically describe vader_sentiment variable and a visualization of the distribution of VADER sentiment scores
  * Create categorical variable of positive, negative, and neutral to visualize overall sentiment trends
  * Investigate negative sentiment reviews (< -0.5) and their associated review scores
  * Evaluate breakdown of books with most recieved negative sentiment reviews
  * Evaluate breakdown of authors with most recieved negative sentiment reviews
  * Explore distribution of each review sentment category with boxplot


## Authors

Contributors names:

* Chetu Barot 
* Adarsh Mohanraju
* Travis Montgomery


## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews
