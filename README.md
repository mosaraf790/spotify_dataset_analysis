
🧭 The EDA Project Briefing
Decoding the DNA of Spotify Hits through Data & Sound Design

This repository contains our team’s submission for The Manhattan Project’s First Exploratory Data Analysis (EDA) challenge — focused on Spotify Music Intelligence.

🎯 Mission Statement:
Analyze Spotify’s vast audio dataset to uncover actionable insights that help artists, producers, and mixing engineers craft commercially optimized, emotionally resonant music.
Our goal: translate sound analytics into creative intelligence — blending music production, listener psychology, and AI-driven data exploration.

🚀 How to Run the Project

To replicate our findings, open the main notebook:
👉 Spotify_EDA.ipynb

Dependencies:

Pandas

Numpy

Matplotlib

Seaborn

Scikit-learn

Joblib

🔍 Key Insights & Findings
🎧 1. The Hit Zone Blueprint

Hit songs consistently fall within these ranges:

Duration: 2.8–3.8 minutes

Tempo: 100–120 BPM (mid-tempo groove)

Loudness: −6 to −8 dBFS (commercial standard)

Danceability: 0.70–0.80

Energy: 0.75–0.85

Valence: 0.55–0.70

➡️ These metrics define the "sweet spot" for modern hits — energetic, rhythmic, and emotionally engaging.

🎤 2. Vocal Dominance & Composition Patterns

Tracks with low instrumentalness and moderate speechiness dominate top popularity scores.

Studio-recorded (low liveness) songs outperform live versions.

Short intros & early hooks significantly increase replay rates.

Key and mode (major/minor) have minimal influence — structure and flow matter more.

🎚️ 3. Mixing & Mastering Guidelines

Maintain loudness between −6 and −8 dBFS for perceived energy without distortion.

Slight compression boosts clarity while retaining dynamic range.

Moderate acousticness yields mainstream polish.

Avoid overly long or low-energy mixes for streaming success.



🎭 Mood Strategy:
Focus on Happy, Excited, or Intense tracks for virality; use Peaceful/Chill tones to sustain long-term listener retention.

🎛️ 5. Groove & Flow Intelligence

Rap & Pop crossovers thrive at 85–105 BPM and 120–135 BPM.

Moderate speechiness (0.3–0.5) increases playlist inclusion.

4/4 time signature dominates — simple, consistent rhythm supports memorability.

📈 6. Trend Evolution (2000–2025)

Time Series Analysis revealed shifting production trends:

Feature	Direction	Interpretation
Danceability	↑	Listeners prefer groove-based tracks
Energy	↓	Softer “chill” production gaining ground
Tempo	↓	Mid-tempo dominates streaming hits
Duration	↓	Shorter songs increase completion rate
Acousticness	↗ (post-2020)	Hybrid acoustic-electronic comeback
Popularity	↑ until 2019	Streaming boom period peak
🧠 7. Algorithmic Optimization Insights

Cold-Start Priors:
Prioritize mid-energy (0.7–0.8), mid-tempo (100–120 BPM), low liveness, and balanced loudness tracks for playlist algorithms.

Hidden Gem Discovery:
Identify low-popularity tracks that already match hit-zone metrics — ideal for editorial or algorithmic resurfacing.

Feature Engineering for Modeling:
Regularize correlated features (e.g., energy–loudness, acousticness–energy), normalize outliers, and winsorize extreme ratios to stabilize model predictions.

🤖 Machine Learning: Popularity Prediction Model

A Random Forest Regressor was trained using the top 9 audio features.

Performance Metrics:

R²: 0.70

MAE: ≈ 4.5

RMSE: ≈ 5.8

Feature Importances:

Energy

Danceability

Loudness

Valence

Acousticness

Tempo

Duration_min

Instrumentalness

Speechiness

➡️ These parameters collectively predict how well a track aligns with mainstream listener preferences.

🧩 Repository Structure
├── README.md                    → Project overview & insights  
├── spotify_tracks.csv           → Primary dataset  
├── spotify_data_description.csv → Column details  
├── Spotify_EDA.ipynb            → Full notebook with analysis & visuals  
├── Spotify Dataset Mindmaps.pdf → Feature context & evaluation  
└── spotify_results/             → Generated outputs & plots


🎶 Conclusion

This project bridges data science and sound design — transforming raw Spotify analytics into creative, actionable insights for artists and producers.
By understanding the evolving trends in tempo, mood, and sonic energy, creators can craft music that resonates both emotionally and algorithmically.

💡 “Data doesn’t kill creativity — it perfects it.”