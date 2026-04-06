# Spotify Tracks Dataset — Audio Features

## Overview

Dataset of Spotify tracks with detailed audio feature metrics. This dataset contains a comprehensive collection of musical tracks from Spotify along with their corresponding audio characteristics and metadata.

- Problem type: Exploratory Data Analysis (EDA)
- Number of records: ~114,000 tracks
- Analysis unit: 1 row = 1 track
- Focus: Audio features, track characteristics, and musical patterns

---

## Key Variables

### 1. Track Information

| Variable | Type | Description |
|----------|------|------------|
| track_id | String | Unique Spotify identifier for the track |
| track_name | String | Name of the track |
| artist_name | String | Name of the artist |
| album_name | String | Name of the album |
| release_date | Date | Release date of the track |

---

### 2. Audio Features

These numeric features describe the acoustic and musical characteristics of each track:

| Variable | Range | Description |
|----------|-------|------------|
| acousticness | 0.0 - 1.0 | Confidence measure of whether the track is acoustic |
| danceability | 0.0 - 1.0 | How suitable a track is for dancing |
| energy | 0.0 - 1.0 | Intensity and activity of the track |
| instrumentalness | 0.0 - 1.0 | Likelihood that a track is instrumental |
| liveness | 0.0 - 1.0 | Presence of live audience during recording |
| loudness | dB | Overall loudness of the track |
| speechiness | 0.0 - 1.0 | Presence of spoken words in the track |
| tempo | BPM | Speed and pace of the track |
| valence | 0.0 - 1.0 | Musical positivity/cheerfulness |
| key | Integer | Tonal center of the track |
| mode | 0/1 | Major (1) or Minor (0) key |
| time_signature | Integer | Number of beats per measure |

---

### 3. Popularity Metrics

| Variable | Type | Description |
|----------|------|------------|
| popularity | 0 - 100 | Track popularity on Spotify (0-100 scale) |
| duration_ms | Integer | Length of the track in milliseconds |

---

## Important Notes

- Real data from Spotify API
- Audio features are normalized and standardized by Spotify
- Values range from 0.0 to 1.0 for most features (except loudness, tempo, duration)
- Some tracks may have missing values in certain features
- Dataset provides a rich understanding of musical characteristics across genres and artists
- Features are pre-computed by Spotify's audio analysis algorithms

---

## Possible Use Cases

- Audio feature distribution analysis across different genres
- Track popularity patterns and their relationship with audio characteristics
- Clustering and segmentation of tracks based on audio features
- Predictive modeling of track success and engagement
- Visualization of musical trends and patterns
- Feature engineering for music recommendation systems
- Principal Component Analysis (PCA) for dimensionality reduction

---

## Analysis Objectives

1. Explore the distribution of audio features
2. Identify patterns and correlations between audio characteristics
3. Analyze relationships between audio features and track popularity
4. Visualize musical characteristics and their trends
5. Discover clustering patterns in music data
6. Provide insights into what makes tracks popular on Spotify