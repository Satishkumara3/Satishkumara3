<div align="center">
  <img src="../assets/banner.svg" alt="Project Banner" width="100%">
  
  # 🎬 Movie Recommendation System
  
  <p>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-Learn" />
    <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
    <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />
  </p>
</div>

## 📖 Overview
The **Movie Recommendation System** utilizes content-based filtering algorithms and Natural Language Processing to suggest movies based on the user's preference. Built with Scikit-Learn and Pandas, the system is wrapped in a dynamic Streamlit frontend to deliver a smooth user experience.

## ✨ Features
- **Personalized Recommendations:** Get 5 similar movies based on what you love.
- **Cosine Similarity:** Uses advanced vector arithmetic to find conceptually similar movie plots and genres.
- **Fast Search & Filter:** Quick predictive search interface.
- **Poster Integration:** Fetches and displays real-time movie posters via TMDB API.

## 🛠️ Tech Stack
- **Machine Learning:** Scikit-Learn
- **Data Engineering:** Pandas, NLTK
- **Vectorization:** CountVectorizer
- **Frontend:** Streamlit

## 📂 Folder Structure
```text
Movie_Recommender/
├── app.py
├── model/
│   ├── similarity.pkl
│   └── movie_list.pkl
├── jupyter/
│   └── model_building.ipynb
├── requirements.txt
└── README.md
```

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Satishkumara3/Movie-Recommendation-System.git
   cd Movie-Recommendation-System
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## 💡 Usage

```bash
streamlit run app.py
```
Navigate to `http://localhost:8501` to start getting recommendations!

## 📸 Screenshots
<div align="center">
  <img src="../assets/ai_background.svg" alt="App Screenshot" width="600">
  <p><i>Recommendation results UI</i></p>
</div>

## 🏗️ Architecture Diagram
```mermaid
graph TD
    A[TMDB 5000 Dataset] --> B(Data Preprocessing - Pandas)
    B --> C(Feature Extraction - NLP tags)
    C --> D[CountVectorizer]
    D --> E[Cosine Similarity Matrix]
    E --> F[Pickle Store]
    F --> G(Streamlit App)
    H[User Input] --> G
    G --> I[Top 5 Movie Matches]
```

## 📊 Results
- **Optimized Latency:** Inference happens instantly relying on the pre-computed similarity matrix.
- Accurately captures nuances between directors, cast, and genres for deep connections.

## 🔮 Future Improvements
- Implement collaborative filtering for user-based recommendations.
- Integrate a database to save user viewings.
- Add an autocomplete search bar for robust typo-handling.

## 📜 License
Provided under the MIT License.

## 🙏 Acknowledgements
- TMDB API
- Streamlit framework
