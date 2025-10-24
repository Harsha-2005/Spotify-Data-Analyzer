Spotify Data Analyzer: Exploratory Data Analysis with Pandas and Matplotlib

Project Overview

This project is a comprehensive **Exploratory Data Analysis (EDA)** of a large Spotify track dataset. It leverages Python's powerful data science ecosystem, specifically **Pandas** for data manipulation and **Matplotlib** (enhanced by **Seaborn**) for visualization, to uncover relationships between song attributes and popularity.

The primary goal of this analysis is to answer questions such as: *What audio characteristics are associated with higher track popularity?* and *What is the distribution of key musical features (e.g., danceability, energy) across the dataset?*


Technologies Used

  * **Python:** The core programming language.
  * **Pandas:** Used for loading the CSV data, cleaning, and manipulation (e.g., duration conversion, grouping).
  * **Matplotlib / Seaborn:** Used for generating high-quality static visualizations (Histograms, Heatmaps, Bar Charts, and Regression Plots).
  * **CSV Files:** The raw data source for the project.


Analysis Highlights

The analysis covers several key areas of the Spotify dataset:

1\. Feature Correlation & Synergy

  * A **Correlation Heatmap** was generated to map the linear relationships between nine core audio features (e.g., `danceability`, `energy`, `loudness`, `acousticness`, and `popularity`).
  * **Key Finding:** A strong positive correlation was identified between **Energy** and **Loudness** (**+0.77**), while **Acousticness** showed a strong inverse relationship with both (**-0.74** for Energy).

2\. Popularity Drivers

  * An investigation into the relationship between individual features and `popularity` was performed using regression plots.
  * **Key Finding:** The highest correlations with popularity were found to be **Loudness** (**+0.31**) and **Energy** (**+0.24**). Overall, popularity distribution is highly skewed, suggesting that high-score tracks are rare outliers.

3\. Track Trends

  * Bar charts were used to visualize the **Top 10 Most Popular Artists** (by average popularity) and the distribution of genres within the dataset.
  * **Data Preparation:** Track duration was converted from milliseconds to a more readable **minutes** format (`duration_min`) for analysis.


 



How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone [Your Repository URL]
    cd spotify-data-analyzer
    ```
2.  **Install Dependencies:**
    ```bash
    pip install pandas matplotlib seaborn
    ```
3.  **Place Data:** Ensure your `dataset.csv` file (or similarly structured Spotify data) is in the root directory.
4.  **Execute the Script:** Run the main analysis script or Jupyter Notebook.
