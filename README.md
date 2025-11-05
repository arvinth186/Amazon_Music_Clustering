# Amazon_Music_Clustering

<h1 align="center">🎵 Amazon Music Clustering Analysis</h1>

<p align="center">
  <b>Unsupervised Learning • Audio Analytics • Data Visualization</b><br>
  Discovering natural groupings of Amazon Music tracks using <b>K-Means Clustering</b>
</p>

---

<h2>📘 Project Overview</h2>

This project performs <b>unsupervised clustering</b> on <b>Amazon Music track data</b> to uncover patterns and categorize songs based on their audio features.  
By analyzing properties like <code>energy</code>, <code>danceability</code>, <code>valence</code>, and <code>acousticness</code>, the project identifies natural music groups such as:
- 🎧 Energetic / Dance tracks  
- 🎶 Acoustic / Chill songs  
- 🎙️ Live or Rap-style tracks  

The insights can help build <b>music recommendation systems</b> or <b>mood-based playlists</b>.

---

<h2>🚀 Objectives</h2>

✅ Explore and preprocess audio feature data  
✅ Apply <b>K-Means clustering</b> to identify song groups  
✅ Visualize and interpret clusters through advanced plots  
✅ Understand how musical features relate to mood or genre  

---

<h2>🧠 Methodology</h2>

<h3>1️⃣ Data Preprocessing</h3>

- Cleaned and normalized dataset using <b>StandardScaler</b>  
- Features include:  
  <code>danceability</code>, <code>energy</code>, <code>loudness</code>, <code>speechiness</code>, <code>acousticness</code>,  
  <code>instrumentalness</code>, <code>liveness</code>, <code>valence</code>, <code>tempo</code>, <code>duration_min</code>  
- Checked for missing values and handled outliers  

<h3>2️⃣ Model Building — K-Means Clustering</h3>

- Experimented with multiple values of <b>k</b>  
- Evaluated cluster performance using:  
  - 📉 <b>Elbow Method</b> (SSE)  
  - 📈 <b>Silhouette Score</b>  
- Optimal cluster count: <b>k = 3</b>  

<h3>3️⃣ Cluster Visualization & Interpretation</h3>

- <b>Boxplots:</b> Feature distribution across clusters  
- <b>Pairplots:</b> Visualized 2D feature relationships  
- <b>Heatmaps:</b> Correlation patterns within each cluster  

---

<h2>🎨 Visual Insights</h2>

<h3>📊 Feature Summary by Cluster</h3>

| Feature | Cluster 0 | Cluster 1 | Cluster 2 |
|----------|------------|-----------|-----------|
| **Danceability** | High | Medium | High |
| **Energy** | Medium | Low | High |
| **Loudness** | Medium | Low | High |
| **Speechiness** | Very High | Low | Low |
| **Acousticness** | Medium | High | Low |
| **Instrumentalness** | Low | Medium | Low |
| **Liveness** | High | Low | Low |
| **Valence** | Moderate | Low | High |
| **Tempo** | Medium | Medium | Slightly High |
| **Duration (min)** | ~3–5 min | ~3–5 min | ~3–5 min |

---

<h3>🧩 Cluster Interpretations</h3>

| Cluster | 🎵 Description | 💬 Example Type |
|----------|----------------|----------------|
| **Cluster 0 (Blue)** | 🎙️ <b>Spoken-word / Rap / Live Tracks</b> <br>High speechiness, moderate energy and loudness. | Rap, live performances, talk-style songs |
| **Cluster 1 (Orange)** | 🎶 <b>Acoustic / Emotional / Chill Songs</b> <br>High acousticness, low energy and valence. | Soft pop, indie, lo-fi, ballads |
| **Cluster 2 (Green)** | 🎧 <b>Energetic / Dance / Happy Songs</b> <br>High energy, loudness, valence, and danceability. | EDM, pop hits, party music |

---

<h3>🔍 Feature Relationships</h3>

- 💥 <b>Energy ↔ Loudness:</b> Strong positive correlation → louder songs are more energetic  
- 🎸 <b>Energy ↔ Acousticness:</b> Negative correlation → acoustic tracks have lower energy  
- 💃 <b>Danceability ↔ Valence:</b> Positive correlation → happier songs are more danceable  

---

<h2>📈 Evaluation Metrics</h2>

- 🧩 <b>Elbow Method:</b> Curve flattened around <code>k = 3</code>  
- 🧠 <b>Silhouette Score:</b> Highest at <code>k = 3</code>, confirming clear separation  

---

<h2>🛠️ Tools & Technologies</h2>

| Category | Tools |
|-----------|-------|
| **Language** | Python 3.x |
| **Libraries** | pandas, numpy, matplotlib, seaborn, scikit-learn |
| **Algorithm** | K-Means |
| **Visualization** | Matplotlib, Seaborn |
| **Environment** | Jupyter Notebook |

---

<h2>📂 Project Structure</h2>

Amazon-Music-Clustering/
│
├── amazon.ipynb # Main analysis notebook
├── README.md # Project documentation
├── dataset/ # Input data (audio features)
├── visuals/ # Output plots & heatmaps
└── requirements.txt # Python dependencies



---

<h2>📚 Key Learnings</h2>

- Audio features effectively capture <b>song mood and similarity</b>.  
- K-Means is powerful for <b>unsupervised song segmentation</b>.  
- Visual analysis (Boxplot, Pairplot, Heatmap) adds <b>explainability</b> to clustering results.  

---

<h2>💡 Future Improvements</h2>

- Integrate <b>PCA</b> for dimensionality reduction and clearer visuals.  
- Try other algorithms: <b>DBSCAN</b>, <b>Gaussian Mixture Models (GMM)</b>.  
- Build a <b>Streamlit or Flask-based web app</b> for interactive recommendations.  
- Connect with <b>Spotify / Amazon Music APIs</b> for live track analysis.  

---

<h2>🧩 Conclusion</h2>

This project demonstrates how <b>unsupervised learning</b> can reveal hidden structures in music data.  
By clustering based on musical attributes, we identified three distinct categories of songs:

- 🎙️ <b>Cluster 0:</b> Spoken-word / Rap / Live  
- 🎶 <b>Cluster 1:</b> Acoustic / Emotional / Chill  
- 🎧 <b>Cluster 2:</b> Energetic / Happy / Dance  

These insights can be leveraged for:
- 🎵 Music recommendation systems  
- 💫 Playlist generation  
- 🎭 Mood-based classification  

---

<h2>👩‍💻 Author</h2>

<b>Arvinth AthiKesav</b>  
🎧 <i>Amazon Music Clustering — Data Science Mini Project</i>  
📬 <b>GitHub:</b> [PriyaRoshini11](https://github.com/PriyaRoshini11)

---

<h4 align="center">⭐ If you like this project, don’t forget to star the repo!</h4>
