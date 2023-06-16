# Movie Recommender
Our Movie Recommendation System is a powerful tool designed to help users discover movies tailored to their preferences and interests. By leveraging basic algorithms and data analysis techniques, our system provides personalized recommendations.

With the number of movies releasing each year, it is easy to miss out on the ones which might align with one’s taste. We have a solution to refine movie-watching experience.

## Process
DATA - Find the relevant data through API, CSV etc
Preprocess - Check and clean the data
Model - Build a relevant model as per the data
Interface - Build an interface to present the results

### Finding the DATA options
Web Scraping - Manually collecting data from different movie database website and streaming platforms
TMDB - API request could be made from TMDB.com
Kaggle - CSV files found with Movie details and another with Cast & Crew

### Preprocessing the DATA
Missing Data - Check if there is any field with missing data
Popular Cast & Crew - Pulled the top 3 cast & director from crew list
Relevant Columns - After the intial check, we decided to drop excess columns 
Duplicate Data - Check if there are duplicate fields
Formatting - Pull data from dictionaries and have all the data in the same format
Creating Tags - Concatenating the Overview, Genre, Keywords, Cast & Crew columns

### Model Building
Vectorization - Scikit Learn library used to easily convert tags word by word to vectors
Stemming - Used NLTK library to Stem the words to their base/root form 
Indexing - Used ‘enumerate’ function to hard code index 
Count Vectorizer - Used CV function to set limit to max words and disregard stop words
Similarity - Used Scikit Learn’s function ‘cosine similarity’ to calculate how similar one movie it to others
Recommend - Created a function to recommend the closest 5 results on basis of vectors

![Jupyter notebook](https://github.com/wase3m/Mid-Term_Project/blob/main/photos/Midterm1.png)

