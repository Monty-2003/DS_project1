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
* Platform: Windows 10, MacOS

## Section 2: A Map of our documentation

* Files (Outline)
  * DATA - Folder
    * DataAppendix.pdf
    * data.md
  * SCRIPTS - Folder
    * modeling.ipynb
    * preprocessing.ipynb
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
  * EDA (Exploratory Data Analysis)
    * books_data
      * Calculate the non-null counts for books data and plot the bar chart for the non-null counts by column
      * Count the occurrences of each publisher and plot the bar chart for the top 10 publishers
      * Count the occurrences of each category and plot the bar chart for the top 10 categories
    * books_reviews
      * Count the top 10 items by price with the method '.nlargest' and plot the respective chart
      * Create a scatter plot of price vs. review score with x being 'book_price' and y being 'score'
      * Count reviews by User_id category and plot the top 10 users by number of reviews
  
* modeling.ipynb
  * Download a cleaned version of books_data and reviews_data (known as books_cleaned.csv and reviews_cleaned.csv)
  * Define and load both datasets in python and return it
  * Establish the categories for the respective datasets with '.info()'
  * Import train_test_split and DecisionTreeRegressor to perform tests
  * Prepare the features (X) and target (y)
  * Create a DataFrame to show feature importance 
  * Evaluate accuracy of the model and calculate accuracy with a 10% tolerance
  * Generate additional metrics, such as mean absolute error and variance 


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
