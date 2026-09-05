# Movie Emotion Analysis
EDA and visualization of emotions in 1500 films (1920–2023)

## About the Dataset
- Source: [Kaggle — Movie Feelings Dataset](https://www.kaggle.com/datasets/yakdemir/movie-feelings-emotion-features-for-1500-films)
- 1500 films reduced to 1473 after cleaning (27 films were missing emotion scores)
- Covers films from 1920 to 2023
- Each film scored on multiple emotions using NLP-based analysis

## Tools Used
- Python, Pandas, Matplotlib, Seaborn
- Jupyter Notebook

## Key Findings

### 1. Hope and Resentment dominate all films
Across all 1473 films, hope and resentment scored significantly higher than all other emotions — with a steep dropoff after resentment(Happiness and Compassion are the emotions that usually appear after the dominant 2). The conclusion here is that most movie plots are built on tension between wanting a big payoff for the audience(hope) and harboring negative feelings towards circumstances surrounding the protagonist or towards the antagonist(resentment).

### 2. Hopeful films rate consistently higher
Films above the average hope score (0.072) rated higher AND more consistently on IMDB. The entire high-hope group sits above the overall average — suggesting hope resonates more deeply with audiences than happiness although Happiness is still a common enough emotion often coming up at 3rd/4th place. Even lower-rated films in the high-hope group outperform the average in the same bucket, suggesting that hope is a reliable indicator of quality rather than an occasional coincidence.

### 3. Happiness ≠ High Ratings
Happiness peaks among films rated 80–90, then declines consistently for films rated 90+. This suggests that highly acclaimed films are not necessarily the happiest. Films such as The Godfather and Schindler’s List offer hope of a satisfying resolution, but are ultimately driven by themes of aspiration, conflict, and struggle rather than feel-good storytelling.

### 4. Emotions shifted after 1980
Pre-1980: Resentment led, Hope followed, particularly in the 1960s

Post-1980: Hope took over as the dominant emotion. Compassion fell out of the top three emotions, replaced by Happiness. This suggests a shift in the emotional profile of films over time, with more recent films showing a greater association with happiness rather than compassion, although they are similar emotions, this might conclude to fantastical themes making a resurgence over films that pull the audience to pour sympathy for real life inspired films or fictional movies.

## Charts

### Correlation Between Emotions and IMDB Rating
<img src="visuals/Correlation%20Heatmap.png" width="700"/>

### Do Hopeful Films Rate Higher?
<img src="visuals/Boxplot%20for%20Correleation%20of%20Hope%20Level%20and%20IMDB%20Rating.png" width="600"/>

### Dominant Emotions by Decade
<img src="visuals/BarPlot%20for%20showing%20the%20top%204%20emotions%20in%20every%20decade.png" width="800"/>

## Conclusions
- Hope is the defining emotion of highly rated cinema for at least 4 decades
- The greatest films balance hope with darkness (despair, resentment) — not pure fantastical happiness
- Cinema shifted from resentment-driven to hope-driven storytelling around 1980
- Disgust is the only emotion observed in the heatmap to be negatively correlated with IMDB ratings
