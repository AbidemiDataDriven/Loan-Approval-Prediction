
---

# Loan Approval Prediction Web Application

A professional **Flask-based Machine Learning web application** that predicts whether a loan application will be **approved or rejected** using a trained **Extreme Gradient Boosting (XGBoost)** model.

This project demonstrates an **end-to-end ML deployment pipeline**, from model inference to a user-friendly web interface.

---
## 🔧 Technologies & Tools

![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-blue)
![Jupyter-Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Scikit-Learn](https://img.shields.io/badge/Libraries-Scikit%E2%80%93Learn-blue)
![GitHub](https://img.shields.io/badge/Environment-GitHub-black)
![OS](https://img.shields.io/badge/OS-Ubuntu-orange)
![DDoS protection](https://img.shields.io/badge/DDoS_Protection-Cloudflare-orange)
![Python version](https://img.shields.io/badge/Python-2.7%20%7C%203.8-blue.svg)
![HTML](https://img.shields.io/badge/Language-HTML-brightgreen)
![JavaScript](https://img.shields.io/badge/Language-JavaScript-orange)
![CSS](https://img.shields.io/badge/Language-CSS-blue)

## 🚀 Project Overview

The application:

* Accepts user input via an HTML form
* Scales the input using a pre-trained `StandardScaler`
* Performs inference using an **Extreme Gradient Boosting model**
* Displays a clear **Approved / Rejected** decision

This project is suitable for:

* ML model deployment demonstrations
* Portfolio projects
* Learning Flask + ML integration

---

## 🧠 Machine Learning Stack

* **Model**: Extreme Gradient Boosting (XGBoost)
* **Preprocessing**: StandardScaler
* **Backend**: Flask
* **Frontend**: HTML (Jinja2 Templates)
* **Language**: Python

---

## 📁 Project Structure

```
loan-prediction-app/
│
├── app.py
├── models/
│   ├── extreme_gradient_boosting.pkl
│   └── scaler.pkl
│
├── templates/
│   └── home.html
│
├── static/
│   └── css/
│
├── requirements.txt
└── README.md
```

---

## ⚙️ How It Works

1. User fills in loan-related features via a web form
2. Data is converted to NumPy array and reshaped
3. Input features are scaled using a saved scaler
4. Model predicts loan approval:

   * `1` → Approved
   * `0` → Rejected
5. Result is rendered back to the UI
<img width="1920" height="1080" alt="Screenshot 2026-06-08 at 2 20 23 AM" src="https://github.com/user-attachments/assets/4a5f0295-4490-4c3f-b766-e396f48bef4d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d05b2ace-0010-44b2-81c5-ded63ce19550" />

---

## 🧩 Core Application Logic

```python
data = [float(x) for x in request.form.values()]
data_np = np.array(data).reshape(1, -1)
scaled_data = scaler.transform(data_np)
prediction = model.predict(scaled_data)[0]
```

---

## ▶️ Running the Application Locally

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/loan-prediction-app.git
cd loan-prediction-app
```

### 2️⃣ Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Start the Flask Server

```bash
python app.py


---

## 👨‍💻 Author

**Abidemi Avoseh**
Machine Learning Engineer & Data Scientist
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abidemi-avoseh-811b7615a/)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/avoseh_emma)

---


## loan Prediction workflow
/Users/abidemiavoseh/Desktop/Screenshot 2025-12-16 at 12.58.44 PM.png
/Users/abidemiavoseh/Desktop/Screenshot 2025-12-16 at 12.59.02 PM.png

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-black?logo=flask&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-ML%20Model-orange)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-ML-yellow?logo=scikitlearn&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)



