Exploring the CMU Movie Corpus: Insights and Analysis

Abstract:
This project allowed me to refine my data analysis skills and explore the power of natural language processing (NLP) by diving into movie data. I applied NLP techniques like sentiment analysis and topic modeling to analyze plot summaries, experimented with linear regression to understand the relationship between movie genres and box office revenue, and built a Random Forest classifier to predict movie runtime categories. This hands-on experience with data manipulation, analysis, and visualization has made me a more adept data analyst.

Objectives and Solutions
Objective 1: Understanding Themes and Sentiment in Movie Plot Summaries
Objective: Utilize NLP techniques to analyze movie plot summaries for common themes and sentiment patterns, and group them based on content similarities.

Methods:

Preprocessing of Plot Summaries:
Lowercasing the text and removing punctuation.
Tokenizing text into individual words.
Removing stopwords (common words like 'and', 'the', etc.).

Sentiment Analysis:
Using the VADER sentiment analysis tool.
Calculating sentiment scores (positive, negative, neutral, compound) for each plot summary.

Theme Identification and Clustering:
Applying TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to represent plot summaries as numerical vectors.
Using the KMeans clustering algorithm to group plot summaries based on their content similarities.
Visualizing clusters with word clouds to identify common themes.

Results:
Clustering plot summaries into groups with distinct themes.
Visualizing word clouds for each cluster, revealing prevalent themes.
Identifying sentiment patterns to understand the emotional tone of movie narratives.


Objective 2: Identifying Revenue-Generating Movie Genres
Objective: Determine which movie genres are more likely to generate higher box office revenue.

Methods:
Linear Regression Analysis:
Exploring the relationship between movie genres and box office revenue.
Converting genres into dummy variables.
Using linear regression to quantify the impact of each genre on box office revenue.

Results:
Identifying genres with the strongest positive and negative correlations with box office revenue.
Gaining insights into which genres are more likely to result in higher or lower box office earnings.
Example: The genre "Revenge" shows a significant positive correlation with box office revenue, suggesting that movies in this genre are more likely to be financially successful.

Objective 3: Classifying Movies by Runtime Categories
Objective: Develop a model to classify movies into different runtime categories (short, medium, long) based on genres, box office revenue, and release year.

Methods:

Feature Engineering:
Categorizing movie runtimes into short, medium, and long categories.
Creating dummy variables for genres.

Random Forest Classifier:
Training a classifier using the Random Forest algorithm.
Utilizing features such as genres, box office revenue, and release year to predict runtime categories.

Results:
Achieving high accuracy in classifying movies into runtime categories.
Demonstrating strong precision, recall, and F1-scores across all categories.

Performance Metrics:
Accuracy: 0.9596
Precision, recall, and F1-scores: All above 0.94 across all categories.

Conclusion:
Through this project, I gained valuable experience in data manipulation, analysis, and visualization. I successfully applied NLP techniques, linear regression, and classification algorithms to extract insights from the CMU Movie Corpus, making me a more skilled data analyst.
