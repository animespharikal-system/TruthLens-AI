# TruthLens AI 🔍

AI-Powered Fake News Detection Platform

TruthLens AI is a full-stack web application that analyzes news articles and predicts whether the content is likely **Real** or **Fake** using Machine Learning and Natural Language Processing techniques.

The platform combines a modern React frontend with a FastAPI backend and a trained text-classification model to provide real-time credibility analysis.

---

## 🚀 Features

* Fake News Detection using Machine Learning
* Real-time News Analysis
* FastAPI REST API Backend
* Modern React + Vite Frontend
* TF-IDF Text Vectorization
* Confidence Score Generation
* Interactive User Interface
* Swagger API Documentation
* Modular Full-Stack Architecture

---

## 🏗️ System Architecture

```text
Frontend (React + Vite)
          │
          ▼
      FastAPI API
          │
          ▼
   Text Preprocessing
          │
          ▼
TF-IDF Vectorization
          │
          ▼
 Machine Learning Model
          │
          ▼
Prediction + Confidence Score
```

---

## 🛠️ Tech Stack

### Frontend

* React
* TypeScript
* Vite
* CSS

### Backend

* FastAPI
* Python
* Pydantic
* Uvicorn

### Machine Learning

* Scikit-Learn
* TF-IDF Vectorizer
* Logistic Regression
* Joblib

### Dataset

* ISOT Fake and Real News Dataset
* Source: Kaggle

---

## 📂 Project Structure

```text
TruthLens-AI
│
├── FakeNews-Frontend
│   ├── src
│   ├── public
│   ├── package.json
│   └── ...
│
├── FakeNews-Backend
│   ├── data
│   ├── models
│   ├── models_ml
│   ├── routes
│   ├── services
│   ├── scripts
│   ├── utils
│   └── main.py
│
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/animespharikal-system/TruthLens-AI.git
cd TruthLens-AI
```

---

## Backend Setup

```bash
cd FakeNews-Backend

python -m venv venv

venv\Scripts\activate

pip install -r requirements.txt
```

### Train Model

```bash
python scripts/train_model.py
```

### Run Backend

```bash
python -m uvicorn main:app --reload
```

Backend runs at:

```text
http://127.0.0.1:8000
```

Swagger Documentation:

```text
http://127.0.0.1:8000/docs
```

---

## Frontend Setup

```bash
cd FakeNews-Frontend

npm install

npm run dev
```

Frontend runs at:

```text
http://localhost:5173
```

---

## API Endpoint

### Predict News

```http
POST /predict
```

Request:

```json
{
  "text": "NASA announced the discovery of a new exoplanet."
}
```

Response:

```json
{
  "prediction": "Real",
  "confidence": 97.3
}
```

---

## 📊 Model Performance

Current Model Metrics:

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 98.53% |
| Precision | 97.88% |
| Recall    | 99.11% |
| F1 Score  | 98.49% |

---

## 🔮 Future Improvements

* Transformer-based Models (BERT/RoBERTa)
* Fact-checking API Integration
* Source Credibility Scoring
* News URL Analysis
* Multilingual Support
* Explainable AI Predictions
* Cloud Deployment

---

## ⚠️ Limitations

This project is intended for educational and research purposes.

Predictions are generated using machine learning patterns learned from historical news datasets and should not be considered absolute verification of factual accuracy.

---

## 👨‍💻 Author

**Animes Pharikal**

Engineering Student | Full Stack Developer | AI Enthusiast

GitHub:
https://github.com/animespharikal-system

---

## 📜 License

MIT License

```
```
