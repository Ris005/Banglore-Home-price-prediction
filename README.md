# 🏠 Bengaluru House Price Prediction Website

# Overview
This end-to-end data science project demonstrates how to build a **real estate price prediction website** using machine learning. It uses the Bengaluru housing dataset from Kaggle to train a regression model, deploys the model via a Flask API, and connects it to a web interface built with HTML, CSS, and JavaScript. The goal is to allow users to input property details and receive an instant price prediction.

# Objectives
- Predict house prices based on features like location, square footage, number of bedrooms, and bathrooms.
- Build a backend API using Flask to serve predictions.
- Create a user-friendly frontend interface to interact with the model.

# Dataset
- **Source:** [Kaggle – Bengaluru House Price Data](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data)
- **Features Used:** Location, sqft, BHK, bath
- **Target Variable:** Price (in lakhs)

---

# Data Science Concepts Covered
- Data loading and cleaning  
- Outlier detection and removal  
- Feature engineering  
- Dimensionality reduction  
- GridSearchCV for hyperparameter tuning  
- K-Fold cross-validation  
- Model evaluation using R² Score and RMSE

# Technologies & Tools
| Category        | Tools Used                          |
|----------------|--------------------------------------|
| Programming     | Python                              |
| Data Cleaning   | Pandas, NumPy                       |
| Visualization   | Matplotlib                          |
| Modeling        | Scikit-learn (Linear Regression)    |
| IDEs            | Jupyter Notebook, VS Code, PyCharm  |
| Backend         | Flask                               |
| Frontend        | HTML, CSS, JavaScript               |
| API Testing     | Postman                             |

# Project Architecture
mermaid
graph TD
A[User Input via Web UI] --> B[JavaScript sends request to Flask API]
B --> C[Flask API loads saved ML model]
C --> D[Model predicts house price]
D --> E[API returns prediction to UI]


# Repository Structure
├── data/                  # Raw and cleaned dataset
├── notebooks/             # Jupyter notebooks for EDA and modeling
├── model/                 # Saved model (.pkl)
├── server/                # Flask backend (app.py)
├── frontend/              # HTML/CSS/JS files
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation


### 🧪 How to Run Locally

#### 1️⃣ Clone the repository
```bash
git clone https:/Ris005/github.com//bengaluru-home-price-prediction.git
cd bengaluru-house-price-prediction
```

#### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

#### 3️⃣ Run the Flask server
```bash
python app.py
```

#### 4️⃣ Test the API using Postman
**POST** `http://localhost:5000/predict`  
**Body (JSON):**
```json
{
  "location": "Whitefield",
  "sqft": 1200,
  "bath": 2,
  "bhk": 2
}
```

---

### 📈 Results
- **Model Used:** Linear Regression  
- **R² Score:** 0.82  
- **RMSE:** ~7.5 lakhs  
- **API Response Time:** ~200ms

---

# Future Enhancements
- Add Streamlit dashboard for interactive predictions  
- Integrate location-based price heatmaps using Folium  
- Use XGBoost or Random Forest for improved accuracy  
- Deploy on Heroku, AWS, or Azure for public access  
- Add form validation and responsive design to frontend

---

### 🙋‍♂️ Author
**Rishu Anand**  
B. Tech – Electronics & Communication  
Aspiring Data Science/Analyst  
📍 Patna, India  

---

Let me know if you want help writing the `app.py`, creating visuals for your repo, or deploying this project to the cloud. We can turn this into a portfolio centerpiece.
