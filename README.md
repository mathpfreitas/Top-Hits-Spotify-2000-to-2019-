# 🎶 Top Hits from Spotify (2000-2019) 🎶

![Spotify Hits](https://img.shields.io/badge/Download%20Dataset-brightgreen?style=for-the-badge&logo=spotify&logoColor=white)

Welcome to the **Top Hits from Spotify (2000-2019)** repository! This dataset offers a rich collection of Spotify music information featuring hit songs spanning from 2000 to 2019. The aim is to explore this data by genre, year, artist, and other musical characteristics.

## 📦 Getting Started

To get started, you can download the dataset from the [Releases section](https://github.com/mathpfreitas/Top-Hits-Spotify-2000-to-2019-/releases). This section contains all the necessary files you need to begin your exploration. 

### 🔍 Purpose of the Dataset

The dataset is designed for music lovers, data analysts, and anyone interested in understanding trends in popular music over nearly two decades. You can analyze:

- **Genres**: Discover which genres dominated the charts.
- **Years**: Track how music trends evolved from 2000 to 2019.
- **Artists**: Identify which artists had the most hits.
- **Musical Characteristics**: Explore various attributes like tempo, danceability, and more.

## 📊 Topics Covered

This repository touches on various topics related to data analysis and visualization, including:

- **Analytics**: Understand the numbers behind the hits.
- **Data Analysis**: Dive deep into the dataset to extract meaningful insights.
- **Data Visualization**: Create charts and graphs to represent your findings visually.
- **Jupyter Notebook**: Utilize Jupyter for interactive data analysis.
- **Matplotlib**: Leverage Matplotlib for creating stunning visualizations.
- **Pandas**: Use Pandas for data manipulation and analysis.
- **Music Trends**: Analyze trends in popular music over the years.

## 📈 Dataset Structure

The dataset consists of several key columns that provide valuable insights:

- **Track Name**: The name of the song.
- **Artist**: The artist or band performing the song.
- **Genre**: The genre of the music.
- **Year**: The year the song was released.
- **Danceability**: A measure of how suitable a track is for dancing.
- **Energy**: A measure of intensity and activity.
- **Loudness**: The overall loudness of a track in decibels (dB).
- **Tempo**: The speed of the music, measured in beats per minute (BPM).

### 📊 Sample Data

Here’s a glimpse of what the dataset looks like:

| Track Name           | Artist           | Genre         | Year | Danceability | Energy | Loudness | Tempo |
|----------------------|------------------|---------------|------|--------------|--------|----------|-------|
| Shape of You         | Ed Sheeran       | Pop           | 2017 | 0.82         | 0.73   | -4.02    | 95.0  |
| Rolling in the Deep   | Adele            | Soul          | 2011 | 0.68         | 0.60   | -5.20    | 105.0 |
| Blinding Lights      | The Weeknd       | Synth-pop     | 2019 | 0.85         | 0.80   | -3.50    | 171.0 |
| ...                  | ...              | ...           | ...  | ...          | ...    | ...      | ...   |

## 🛠️ Tools and Libraries

For your analysis, you can use the following tools and libraries:

- **Python**: The main programming language for data analysis.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For data visualization.
- **Jupyter Notebook**: For an interactive coding environment.

### 📚 Installation

Make sure you have Python installed. You can download it from the [official Python website](https://www.python.org/downloads/).

After installing Python, you can set up your environment:

```bash
pip install pandas matplotlib
```

## 📊 Visualization Examples

Visualizing data can provide deeper insights. Here are some examples of what you can create with this dataset:

### 1. Genre Distribution

You can create a pie chart to visualize the distribution of genres in the dataset.

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
data = pd.read_csv('spotify_hits.csv')

# Count genres
genre_counts = data['Genre'].value_counts()

# Plot
plt.figure(figsize=(10, 6))
genre_counts.plot(kind='pie', autopct='%1.1f%%')
plt.title('Genre Distribution of Top Hits (2000-2019)')
plt.ylabel('')
plt.show()
```

### 2. Yearly Trends

A line graph can help illustrate how the number of hits per year has changed.

```python
# Count hits by year
yearly_hits = data['Year'].value_counts().sort_index()

# Plot
plt.figure(figsize=(10, 6))
yearly_hits.plot(kind='line', marker='o')
plt.title('Number of Hits by Year (2000-2019)')
plt.xlabel('Year')
plt.ylabel('Number of Hits')
plt.grid()
plt.show()
```

### 3. Energy vs. Danceability

You can create a scatter plot to explore the relationship between energy and danceability.

```python
# Scatter plot
plt.figure(figsize=(10, 6))
plt.scatter(data['Danceability'], data['Energy'], alpha=0.5)
plt.title('Energy vs. Danceability of Top Hits')
plt.xlabel('Danceability')
plt.ylabel('Energy')
plt.grid()
plt.show()
```

## 🔄 Updating the Dataset

We plan to keep this dataset updated. To get the latest version, check the [Releases section](https://github.com/mathpfreitas/Top-Hits-Spotify-2000-to-2019-/releases) regularly.

## 🤝 Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to create a pull request or open an issue. 

### How to Contribute

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes.
4. Commit your changes.
5. Push to the branch.
6. Create a pull request.

## 📝 License

This dataset is shared under the MIT License. Feel free to use it for personal or educational purposes.

## 🌟 Acknowledgments

Special thanks to Spotify for providing a rich dataset that allows us to explore the world of music. 

## 📬 Contact

For any questions or suggestions, feel free to reach out. You can contact me through GitHub.

## 🚀 Conclusion

Dive into the world of music from 2000 to 2019. Use this dataset to explore, analyze, and visualize the trends that shaped the music industry. Download the dataset from the [Releases section](https://github.com/mathpfreitas/Top-Hits-Spotify-2000-to-2019-/releases) and start your journey today!