Exploring the CMU Movie Corpus: Insights and Analysis

Abstract-

This project served as a practical playground for me to refiine my data analysis skills and explore the power of natural language processing (NLP).

I delved into movie data, using NLP techniques like sentiment analysis and topic modeling to analyze plot summaries. This allowed me to experiment with text processing and gain insights into thematic trends and emotional tones within movies.

Further, I leveraged machine learning through linear regression. This allowed me explore the relationship between movie genres and box office revenue, fostering an understanding of how linear regression works.

Finally, I build a Random Forest classifier to predict movie runtime categories based on features like genre and box office revenue. This exercise strengthens my grasp of feature engineering and classification techniques.

Throughout this project, I had gain hands-on experience with data manipulation, analysis, and visualization, making me a more adept data analyst.

Questions,Methods and Results

Q1: How can natural language processing techniques be leveraged to analyze movie plot summaries for common themes and sentiment patterns, ultimately grouping them based on content similarities?

Methods:

1. Preprocessing of Plot Summaries:  
     
   - Lowercasing the text and removing punctuation.  
   - Tokenization of text into individual words.  
   - Removal of stopwords (common words like 'and', 'the', etc.).

   

1. Sentiment Analysis:  
     
   - Utilization of the VADER sentiment analysis tool.  
   - Calculation of sentiment scores (positive, negative, neutral, compound) for each plot summary.

   

1. Theme Identification and Clustering:  
     
   - TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to represent plot summaries as numerical vectors.  
   - KMeans clustering algorithm to group plot summaries based on their content similarities.  
   - Visualization of clusters using word clouds to identify common themes.

Results:

1. Clustering of plot summaries into groups with distinct themes

\[('one', 31242), ('back', 24465), ('two', 21755), ('film', 20319), ('tells', 19109), ('father', 18553), ('man', 18245), ('time', 17331), ('love', 17242), ('new', 17180), ('life', 17161), ('get', 17135), ('home', 16747), ('also', 16354), ('find', 16133), ('however', 16017), ('house', 15942), ('finds', 15732), ('family', 15612), ('later', 15599)\] Clustering Analysis Results: wiki\_movie\_id  cluster 0       23890098        1 1       31186339        4 2       20663735        4 3        2231378        2 4         595909        4 . 2\. Visualization of word clouds for each cluster, providing insights into the prevalent themes within each group. 3\. Identification of sentiment patterns within plot summaries, aiding in understanding the emotional tone of the movies' narratives.

Q2: Which movie genres are more likely to generate higher box office revenue?

Methods:

1. Linear Regression Analysis:  
   - Investigation of the relationship between movie genres and box office revenue.  
   - Conversion of genres into dummy variables.  
   - Utilization of linear regression to quantify the impact of each genre on box office revenue.

Results:

1. Identification of genres with the strongest positive and negative correlations with box office revenue.  
1. Insights into which genres are more likely to lead to higher or lower box office earnings.

Genre   Coefficient 351                     genre\_ "/m/0bbc17": "Gross out"  1.558033e+14 877                     genre\_{"/m/0bbc17": "Gross out"  1.553680e+14 154   genre\_ "/m/02z8vz": "The Netherlands in World ...  2.106480e+12 137               genre\_ "/m/02rcm2r": "Sponsored film"  1.064812e+12 300                    genre\_ "/m/070yc": "Space opera"  4.633816e+08

The coefficient indicates the strength and direction of the relationship between the genre and the target variable. Positive coefficients suggest a positive relationship, while negative coefficients suggest a negative relationship. The magnitude of the coefficient indicates the strength of the relationship.For example:

The genre "Revenge" has a coefficient of approximately 4.009030e+14, indicating a positive relationship with the target variable. the analysis provides insights into which movie genres are more likely to generate higher box office revenue based on their coefficients.

Q3: Can we classify movies into different runtime categories (short, medium, long) based on their genres and other metadata such as box office revenue and release year?\*\*

Methods:

1. Feature Engineering:  
     
   - Categorization of movie runtimes into short, medium, and long categories.  
   - Creation of dummy variables for genres.

   

1. Random Forest Classifier:  
     
   - Training a classifier using Random Forest algorithm.  
   - Utilization of features such as genres, box office revenue, and release year to predict runtime categories.

Results: Accuracy: 0.9596330275229358 precision    recall  f1-score   support

    long       0.95      0.92      0.94       521

  medium       0.93      0.96      0.95       626

   short       1.00      1.00      1.00       488

accuracy                           0.96      1635

macro avg       0.96      0.96      0.96      1635 weighted avg       0.96      0.96      0.96      1635

1. High accuracy achieved in classifying movies into runtime categories.  
1. Strong precision, recall, and F1-scores across all categories, indicating the effectiveness of the model in predicting movie runtime based on metadata.

The code classifies movies into runtime categories (short, medium, long) based on genres, box office revenue, and release year. It preprocesses the data by creating dummy variables for genres, imputing missing values, and standardizing features. The model is trained using a Random Forest Classifier with hyperparameter tuning via RandomizedSearchCV. The resulting model achieves high accuracy (96.33%) and strong precision, recall, and F1-scores across all categories, demonstrating its effectiveness in predicting movie runtime categories based on the provided metadata.  
