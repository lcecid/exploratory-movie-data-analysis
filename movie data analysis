# Importing pandas and matplotlib
import pandas as pd
import matplotlib.pyplot as plt

# Read in the Netflix CSV as a DataFrame
netflix_df = pd.read_csv("netflix_data.csv")

#Create DataFrame subset for 1990s movies
movies_90 = netflix_df[(netflix_df["release_year"] >= 1990) & (netflix_df["release_year"] < 2000)]
print(movies_90)

#Create histogram for finding an estimate max frequent movie duration
plt.hist(movies_90["duration"])
duration = int(90)

#Create DataFrame subset for action genre movies within 1990s
movies_action_90 = movies_90[(movies_90["genre"] == "Action")]
print(movies_action_90)

#Find the number of movies action genre movies within 1990s
short_movie_count = 0
for index, row in movies_action_90.iterrows():
    if row["duration"] < 90:
        short_movie_count += 1
    else:
        short_movie_count = short_movie_count
print(short_movie_count)
