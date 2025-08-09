# 📌ML Insurance Premium  Predictor

An **end-to-end machine learning application** that predicts an individual's **insurance premium category** based on personal and lifestyle details.  
This single Python file contains **FastAPI backend** for predictions and **Streamlit frontend** for user interaction.

---

## 🚀 Features
- **All-in-One Python Script** – FastAPI + Streamlit in a single file.  
- **Pickle-based Model Loading** – No , uses Python's built-in `pickle` module.  
- **User-Friendly Web UI** built with Streamlit.  
- **Real-time Prediction** based on age, weight, height, income, smoking habits, city, and occupation.  
- **Confidence Score** and **Class Probabilities** displayed.  
- **Deployable Anywhere** (AWS, Azure, Heroku, etc.).  

---

## 🛠 Tech Stack
**Frontend:**  
- Streamlit  

**Backend:**  
- FastAPI  
- Pickle (model loading)  
- scikit-learn (ML model)  

---

## 📂 Project Structure

📁 insurance-premium-predictor
├── app.py # All-in-one API + UI
├── model.pkl # Saved ML model (Pickle format)
├── frontend.py # Streamlit UI code
├── requirements.txt # Dependencies
└── README.md # Documentation 


---

## ⚙️ How It Works
1. User enters their details in Streamlit UI.  
2. Data is sent to FastAPI `/predict` endpoint.  
3. Model predicts the insurance premium category.  
4. UI displays prediction, confidence, and probability distribution.  

---

## 📦 Installation & Usage

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/insurance-premium-predictor.git
cd insurance-premium-predictor

2️⃣ Install dependencies
  pip install -r requirements.txt

3️⃣ Run the application (API + UI)
  Streamlit run app.py

📊 Example API Request
   #POST http://127.0.0.1:8000/predict
    {
  "age": 30,
  "weight": 65.0,
  "height": 1.7,
  "income_lpa": 10.0,
  "smoker": true,
  "city": "Mumbai",
  "occupation": "private_job"
}
   
  # Response 
    {
  "response": {
    "predicted_category": "High",
    "confidence": 0.82,
    "class_probabilities": {
      "0": 0.05,
      "1": 0.13,
      "2": 0.82
    }
  }
}

📜 License
MIT License

---

If you want, I can also **add GitHub badges + a screenshot preview** to make your README look professional and appealing.  
Do you want me to make that polished version?



   


