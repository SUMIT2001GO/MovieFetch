# Movie Recommendation System

![Movie Recommendation System](https://img.shields.io/badge/Streamlit-Movie_Recommendation_System-blue)

## Description

This is a **Movie Recommendation System** built using **content-based filtering**. The system recommends movies similar to the movie selected by the user based on attributes such as **genres**, **keywords**, **cast**, and **crew**. It leverages **cosine similarity** to calculate how similar the movies are based on these features. This is done using a dataset from **The Movie Database (TMDb)**, which contains rich metadata about movies.

**Live Demo**: [Movie Fetch](https://moviefetchsumit007.streamlit.app/)

---

## Table of Contents
1. [Business Objective](#business-objective)
2. [Features](#features)
3. [How It Works](#how-it-works)
4. [Technologies Used](#technologies-used)
5. [Installation](#installation)
6. [How to Use](#how-to-use)
7. [Future Improvements](#future-improvements)
8. [Acknowledgements](#acknowledgements)

---

## Business Objective

The main goal of this Movie Recommendation System is to provide users with personalized movie suggestions based on a movie they already enjoy. By offering personalized content recommendations, this system improves the user experience, engagement, and content discovery.

- **Enhance User Experience**: Helps users discover movies they are more likely to enjoy without sifting through large databases.
- **Increase User Retention**: Personalized movie suggestions lead to better user engagement and longer interaction times with the platform.
- **Content Discovery**: Makes it easier for users to explore new movies they may not have encountered otherwise.

---

## Features

- **Content-Based Recommendations**: Recommends movies similar to the selected movie based on shared genres, keywords, cast, and crew.
- **Simple UI**: A user-friendly interface built with Streamlit allows users to easily search for movies and view recommendations.
- **Movie Posters**: Displays movie posters alongside their names for a more engaging experience.

---

## How It Works

1. **Data Preprocessing**: The model starts by loading movie data from TMDb, which includes movie titles, overviews, genres, keywords, cast, and crew.
   
2. **Feature Extraction**: Relevant features like genres, keywords, and cast are extracted from the data, and the **content-based approach** is used to generate a recommendation.

3. **Cosine Similarity**: The system calculates the cosine similarity between the selected movie and all other movies based on the feature vectors, identifying the most similar movies.

4. **Movie Recommendations**: The top 5 most similar movies are recommended to the user with their corresponding posters for easy identification.

---

## Technologies Used

- **Streamlit**: For creating the interactive web application.
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For calculating cosine similarity between movies.
- **Requests**: To fetch movie posters from an external API.
- **TMDb API**: For fetching movie poster images based on movie IDs.
- **Pickle**: To save and load preprocessed data and model for efficient reuse.

---

## Installation

To run this project locally, follow these steps:

### Prerequisites:
- Python 3.x
- Required Python packages

### Steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/SUMIT2001GO/MovieFetch.git
   cd movie-recommendation-system
   pip install -r requirements.txt
   streamlit run app.py

   
### How to Use:
- Launch the Streamlit app by running streamlit run app.py after installation.
- On the homepage, select a movie from the dropdown list.
- Click on the "Recommend" button.
- View the top 5 recommended movies along with their posters.


![Screenshot 2024-11-07 005057](https://github.com/user-attachments/assets/15b15bed-94f8-4da7-b625-c47fddc47832)



![Screenshot 2024-11-07 005007](https://github.com/user-attachments/assets/82a2af5a-6549-482d-ab15-98e098209a90)




### Future Improvements:
- **Collaborative Filtering**: In addition to content-based filtering, collaborative filtering can be implemented to improve recommendations by considering users' preferences.
- **Better UI/UX**: Enhance the user interface with more interactive and customizable options.
- **User Ratings**: Implement user-based ratings to personalize recommendations even further.

### Acknowledgements:
- **TMDb API**: For providing the movie dataset and poster images.
- **Streamlit**: For the easy-to-use framework to build the web app.
- **Scikit-learn**: For providing the necessary tools to compute cosine similarity and handle machine learning operations.

