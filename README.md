# Recommendation-System
A recommendation system using FastAPI and collaborative filtering to suggest movies, products, or content. Supports user ratings, genre/category-based filtering, and personalized suggestions. Includes REST API endpoints with Swagger UI, runnable on Colab with ngrok.

# 🎬🛍 Recommendation System (FastAPI + Collaborative Filtering)

This project is a **recommendation engine** built with **FastAPI** and **machine learning collaborative filtering**. It provides personalized recommendations for **movies, products, or content** based on user ratings and categories.

---

## 🚀 Features
- User-based collaborative filtering
- Recommendations by genre or product category
- REST API endpoints:
  - `GET /movies` → list movies
  - `GET /products` → list products
  - `POST /rate` → add user ratings
  - `GET /recommend/{user_id}` → get personalized recommendations
- Swagger UI for testing (`/docs`)
- Sample demo users and items included

---

## 🛠 Tech Stack
- **FastAPI** → REST API
- **Pandas, Scikit-learn** → Collaborative filtering
- **SQLite** → Data persistence
- **ngrok** → Public URL on Google Colab

---

## ▶️ Run on Google Colab
1. Upload the notebook (`recommendation_system_colab.ipynb`) to Colab.  
2. Install dependencies:
   ```bash
   !pip install fastapi uvicorn pyngrok nest_asyncio scikit-learn pandas

---

## Apply nest_asyncio and start the FastAPI app in a background thread.
## Connect with ngrok:

from pyngrok import ngrok
ngrok.set_auth_token("YOUR_NGROK_TOKEN")
print(ngrok.connect(8000).public_url)

## Open the printed URL → /docs to explore API.
