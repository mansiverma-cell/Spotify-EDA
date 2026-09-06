# Spotify-EDA

Exploratory Data Analysis of Spotify tracks using Python, Pandas, Matplotlib and Seaborn.

## Dataset
- 113,999 rows × 20 columns (post-cleaning)
- Source: [add Kaggle dataset link here]

## What This Project Covers
- Data cleaning and preprocessing
- Univariate analysis of track features
- Correlation analysis between audio features
- Popularity deep-dive: what drives a track's popularity score
- Genre and artist-level analysis
- Explicit vs. non-explicit content comparison
- Feature engineering

## Key Insights

**1. Audio Features**
Individual audio features such as energy, danceability, loudness, valence, and tempo show very weak relationships with track popularity. No single audio characteristic strongly determines how popular a track becomes.

**2. Genre**
Average popularity varies substantially across genres. Pop-film has the highest average popularity (~59.28), while Iranian has the lowest (~2.21) — a difference of more than 57 points. K-pop is also among the highest-ranked genres (~56.95).

**3. Artist**
Among artists with at least 10 tracks, Bad Bunny has the highest average popularity (~87.1). However, artist track count itself shows no clear relationship with average popularity — artists with fewer tracks show a wider range, while artists with more tracks tend to be more stable.

**4. Explicitness**
The relationship between explicitness and popularity differs substantially across genres. Non-explicit tracks are more popular in genres like K-pop and hip-hop, while explicit tracks are more popular in genres like soul, J-idol, and country — explicitness alone doesn't determine popularity; it's genre-dependent.

**5. Duration & Instrumentalness**
Very long tracks (20+ minutes) mostly fall below 50 popularity. Tracks with higher instrumentalness also tend to have lower popularity. Neither characteristic alone explains popularity fully.

## Conclusion
Spotify track popularity cannot be explained by a single audio feature. Most audio features show very weak relationships with popularity, while genre and artist show much larger differences. The relationship between explicitness and popularity also shifts across genres. Overall, popularity is influenced by multiple, interacting factors rather than one simple characteristic — making it a complex, context-dependent outcome.

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn

## Files
- `Spotify_EDA.ipynb` — full analysis notebook
- `spotify-tracks-dataset.csv` — dataset used
