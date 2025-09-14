# 🏠 Airbnb Price Prediction – London Listings (ML Project)

A real-world machine learning project that predicts nightly prices of Airbnb listings in London using a combination of tabular, textual, sentiment, and spatial features. This was developed as a collaborative team project during our studies at the University of Göttingen.

## 🔍 Problem Statement
To help hosts set optimal prices for their listings, we built a regression model trained on cleaned Airbnb data (~60,000 entries) from the [Inside Airbnb Open Data Initiative](http://insideairbnb.com/get-the-data.html).

## 📦 Dataset
- Source: Inside Airbnb – London
- Size: ~60,000 records after preprocessing
- Target: `price` (converted to float, log-transformed)

## ✨ Features Used
- **Tabular**: Bedrooms, bathrooms, room type, host duration
- **Text**: Listing name, description, neighborhood overview
- **NLP Embeddings**: MiniLM (384-d vectors)
- **Sentiment**: Review sentiment scores
- **Amenities**: Top 50 one-hot encoded
- **Temporal**: Days since last review, host start date

## 🧠 Models Trained
- XGBoost
- CatBoost (Best Performer: MAE = 17.14, R² = 0.8882)
- SVR
- MLP (Neural Network)

## 🛠️ Tech Stack
- Python, Pandas, NumPy
- Scikit-learn, XGBoost, CatBoost
- SentenceTransformers (MiniLM)
- Matplotlib, Seaborn

## 📈 Model Performance
| Model      | MAE   | R²    |
|------------|-------|-------|
| CatBoost   | 17.14 | 0.8882 |
| XGBoost    | ~18   | ~0.85  |
| SVR        | ~19   | ~0.82  |
| MLP        | ~20   | ~0.80  |

## 🧪 Future Improvements
- Incorporate image features (e.g., listing photos)
- Use geo-clustering for better location encoding
- Build API for dynamic price suggestions

## 👨‍💻 Contributors
- Sunil Kumar Nallani
- Mohamed Reda Arsalane
- Mohamed Bilal Abdenouri

## 📂 Repository Structure

