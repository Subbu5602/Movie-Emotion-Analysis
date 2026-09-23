# Movie Emotion Analysis
EDA and visualization of emotions in 1500 films (1920–2023)

> **Problem Statement:** Does the emotional profile of a film's plot predict its IMDB rating — and do critics and audiences respond to different emotions when rating movies?

## About the Dataset
- Source: [Kaggle — Movie Feelings Dataset](https://www.kaggle.com/datasets/yakdemir/movie-feelings-emotion-features-for-1500-films)
- 1500 films reduced to 1473 after cleaning (27 films were missing emotion scores)
- Covers films from 1920 to 2023
- Each film scored on multiple emotions using NLP-based analysis
- The 2020s contain only 53 films, so trends for this decade should be interpreted with caution due to the smaller sample size

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

Post-1980: Hope took over as the dominant emotion. Compassion fell out of the top three emotions, replaced by Happiness. This suggests a shift in the emotional profile of films over time, with more recent films showing a greater association with happiness rather than compassion, although they are similar emotions, suggesting that fantastical themes made a resurgence over films that pull the audience to pour sympathy for real life inspired films or fictional movies.

### 5. Hope leads in plot feeling ratings
Among dominant plot feelings with 50+ films, hope-led films rate highest (75.92) 
while surprise-led films rate lowest (71.65). Bravery is the most common plot feeling 
but sits in the mid-range of average ratings - thus frequency doesn't equal quality.

### 6. Critics and audiences diverge on hope
Both value resentment and compassion similarly, but audiences reward hope 
significantly more than critics (0.19 vs 0.075). Critics lean toward darker 
emotions — sadness and despair correlate stronger with Metascore ratings than IMDB ratings.

## Charts

### Correlation Between Emotions and IMDB Rating
<img src="visuals/Correlation%20Heatmap.png" width="700"/>

### Do Hopeful Films Rate Higher?
<img src="visuals/Boxplot%20for%20Correleation%20of%20Hope%20Level%20and%20IMDB%20Rating.png" width="600"/>

### Dominant Emotions by Decade
<img src="visuals/BarPlot%20for%20showing%20the%20top%204%20emotions%20in%20every%20decade.png" width="800"/>

### Average IMDB Rating by Dominant Plot Feeling
<img src="visuals/Average%20Rating%20by%20Major%20Plot%20Feeling.png" width="700"/>

### What Do Critics vs Audiences Value?
<img src="visuals/Critics%20VS%20Audience.png" width="700"/>

## Conclusions
- Hope is the defining emotion of highly rated cinema for at least 4 decades
- The greatest films balance hope with darkness (despair, resentment) — not pure fantastical happiness
- Cinema shifted from resentment-driven to hope-driven storytelling around 1980
- Disgust is the only emotion observed in the heatmap to be negatively correlated with IMDB ratings
- Films with Hope as the dominant plot feeling rate highest among all dominant plot feelings
- Audiences reward hope significantly more than critics, who lean toward darker emotions like sadness and despair for ratings
