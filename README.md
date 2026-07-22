# crop-recommendation
# 🌾 AgriGPT: AI Crop Recommendation Chatbot

AgriGPT is an intelligent crop recommendation chatbot powered by Machine Learning and Large Language Models (LLMs). It predicts the most suitable crop based on soil nutrients and environmental conditions, then explains the recommendation in natural language with farming advice.

The project combines **XGBoost**, **Google Gemini/OpenAI**, and a structured agricultural knowledge base to provide accurate, explainable, and farmer-friendly recommendations.

---

## 🚀 Features

- 🌱 AI-powered crop recommendation
- 🤖 Natural language chatbot
- 📊 XGBoost Machine Learning model
- 🧠 Top-3 crop predictions with confidence scores
- 🌍 Farmer-friendly explanations
- 💧 Water requirement recommendations
- 🌿 Fertilizer recommendations
- 🌦 Weather-aware recommendations (Future)
- 📈 Feature importance visualization
- 💬 Interactive chat interface
- ☁️ Google Colab compatible

---

## 📌 Problem Statement

Choosing the right crop is one of the biggest challenges for farmers. Crop selection depends on multiple factors including:

- Nitrogen (N)
- Phosphorus (P)
- Potassium (K)
- Temperature
- Humidity
- Soil pH
- Rainfall

Many farmers rely on traditional experience, which may not always produce the best yield.

AgriGPT uses Machine Learning to analyze these parameters and recommend the most suitable crop while providing easy-to-understand explanations.

---

## 🏗 Project Architecture

```
User
   │
   ▼
Chat Interface
   │
   ▼
Input Parser
   │
   ▼
Feature Extraction
   │
   ▼
Data Validation
   │
   ▼
XGBoost Model
   │
   ▼
Top-3 Crop Prediction
   │
   ▼
Confidence Score
   │
   ▼
Knowledge Base
   │
   ▼
Gemini/OpenAI
   │
   ▼
AI Recommendation
```

---

## 🧠 Machine Learning Model

Algorithm:

- XGBoost Classifier

Hyperparameters:

- Learning Rate: 0.03
- Max Depth: 8
- Number of Trees: 500
- Subsample: 0.9
- Column Sample: 0.9
- Gamma: 0.1
- Min Child Weight: 2
- Objective: Multi-class Classification

---

## 📊 Dataset

The project uses the **Crop Recommendation Dataset** containing agricultural and environmental parameters.

### Features

- Nitrogen
- Phosphorus
- Potassium
- Temperature
- Humidity
- Soil pH
- Rainfall

Target:

- Recommended Crop

---

## 📂 Project Structure

```
AgriGPT/

│── AgriGPT.ipynb
│── crop_recommendation.csv
│── crop_model.pkl
│── label_encoder.pkl
│── crop_database.json
│── requirements.txt
│── README.md
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/sakina Khan/AgriGPT.git
```

Navigate into the project

```bash
cd AgriGPT
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## 📦 Required Libraries

- Python 3.10+
- pandas
- numpy
- scikit-learn
- xgboost
- matplotlib
- seaborn
- joblib
- google-generativeai (or OpenAI SDK)

---

## 🚀 Workflow

1. Load Dataset
2. Data Cleaning
3. Exploratory Data Analysis
4. Feature Engineering
5. Train-Test Split
6. Train XGBoost Model
7. Hyperparameter Tuning
8. Model Evaluation
9. Save Model
10. Load Model
11. Predict Crop
12. Generate AI Response

---

## 💬 Example

### User Input

```
Nitrogen: 90
Phosphorus: 42
Potassium: 43
Temperature: 25°C
Humidity: 82%
pH: 6.5
Rainfall: 210 mm
```

### Prediction

```
🌾 Recommended Crop

Rice

Confidence:
98.4%
```

### AI Recommendation

```
Rice is the most suitable crop because your soil contains
sufficient nitrogen, adequate rainfall, high humidity,
and an ideal pH level. Maintain consistent irrigation
and apply balanced NPK fertilizer during the vegetative stage
for better yield.
```

---

## 📈 Model Evaluation

Performance metrics include:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report
- Feature Importance

---

## 🌟 Future Improvements

- Weather API Integration
- Voice Assistant
- Multi-language Support
- Soil Health Analysis
- Fertilizer Optimization
- Yield Prediction
- Market Price Forecasting
- Disease Detection
- Pest Identification
- Mobile Application
- Offline Prediction
- GPS-Based Crop Recommendation

---

## 🛠 Tech Stack

### Machine Learning

- XGBoost
- Scikit-learn

### AI

- Google Gemini API / OpenAI API

### Data Processing

- Pandas
- NumPy

### Visualization

- Matplotlib
- Seaborn

### Deployment

- Google Colab
- Streamlit
- Hugging Face Spaces

---

## 📄 License

This project is developed for educational and research purposes.

---

## 👨‍💻 Author

Developed by **Sakina Khan**

Bachelor of Science in Computer Science

University of Sindh

Machine Learning & AI Enthusiast

---

⭐ If you found this project useful, consider giving it a star on GitHub!
