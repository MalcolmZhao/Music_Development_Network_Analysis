# Music Development Network Analysis

This repository contains the code and data for our project on analyzing the influence relationship between musicians using neural networks.

## Project Structure

- Data: this folder should focus on 2 datasets:
  - `full_music_data.csv`: This dataset includes 16 variable entries for 98,340 songs. These variables include attributes like danceability, tempo, loudness, key, and artist information (name, id, etc.).
  - `influence_data.csv`: This dataset covers musical features for 5,854 artists spanning the last 90 years. It provides both influencing artists and their respective followers.

- `1.music_data_manipulation.ipynb`: This Jupyter notebook is used to manipulate and preprocess the music data. Key steps include matching musician IDs, cleaning the data, and preparing it for feature engineering and model training.
- `2.musician_sequential_input_gen.ipynb`: This notebook is crucial for feature engineering. It generates independent variables by selecting 20 songs per artist in chronological order, creating a sequential representation of each artist's music. These sequential inputs are vital for capturing the temporal and stylistic progression of an artist’s work, enabling the model to effectively assess influence patterns.
- `3.musician_influence.ipynb`: This notebook is used to train the final model. The model is based on TensorFlow and aims to analyze and predict the influence relationships between different musicians.
- `influence_musicians8570.h5`: This file contains the final model weights, trained to evaluate the influence relations.
- `IEOR242-Project-Group6-Statistical Analysis on Music Influence Relation with Neural Network.pdf`: The comprehensive report detailing our analysis, methodologies, results, and conclusions.

## Dependencies
To run the code in this repository, you will need the following Python packages:
- Python 3.7 or higher
- `tensorflow`
- Other dependencies as listed in individual scripts
