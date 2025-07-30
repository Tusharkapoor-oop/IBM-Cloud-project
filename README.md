# 🔧 Predictive Maintenance with Machine Learning on IBM Cloud

An end-to-end AI solution for predicting industrial machine failures using real-time sensor data. Developed, trained, and deployed entirely on **IBM Watsonx.ai**, this project demonstrates how cloud-based machine learning can drive intelligent, proactive maintenance strategies in modern manufacturing.

---

## 📌 Project Objective

Industrial equipment is susceptible to unexpected failures such as **tool wear**, **power outages**, and **thermal issues**. These incidents often result in unplanned downtime, reduced productivity, and financial losses.

This project builds a **predictive maintenance model** capable of forecasting specific failure types before they occur. By analyzing historical and real-time sensor data, the system enables **data-driven, proactive maintenance** rather than reactive repair.

---

## 🚀 Key Highlights

- ✅ Trained a high‑accuracy **Random Forest Classifier** to predict failure types  
- 🧠 Built using **Python**, **Scikit‑learn**, and **Watsonx.ai Notebooks**  
- ☁️ Deployed on **IBM Watsonx.ai Runtime** as a **RESTful API**  
- 🧾 Supports live JSON input for real-time sensor‑based predictions  
- 📦 Scalable cloud pipeline with secure storage via **IBM Cloud Object Storage**

---

## 🛠️ Tech Stack

| Component             | Technology                                     |
|-----------------------|-------------------------------------------------|
| Cloud Infrastructure  | IBM Cloud (Free Tier)                          |
| Model Development     | IBM Watsonx.ai Studio (Notebooks + AutoAI)     |
| Model Deployment      | IBM Watsonx.ai Runtime (API endpoint)          |
| Storage               | IBM Cloud Object Storage                       |
| Language & Libraries  | Python, Pandas, NumPy, Scikit‑learn, Matplotlib |
| Dataset               | Kaggle: Predictive Maintenance Dataset          |

---

## 📁 Project Structure
``
predictive-maintenance-ibm/
├── data/
│   └── sensor_data.csv             # Original dataset from Kaggle
├── notebooks/
│   └── training_pipeline.ipynb     # Data cleaning, EDA, model training
├── model/
│   └── rf_classifier.pkl           # Exported trained model
├── deployment/
│   └── deployment_config.json      # Watsonx Runtime deployment config
├── utils/
│   └── preprocess.py               # Feature engineering utilities
├── README.md
└── requirements.txt




---

## 🧠 ML Pipeline Overview

- **Algorithm:** Random Forest Classifier  
- **Features:** Torque, Voltage, Temperature, Vibration, Rotational Speed  
- **Target Classes:** Tool Wear, Heat Failure, Power Failure, No Failure  
- **Performance:**  
  - Accuracy: ~91%  
  - Evaluated with Confusion Matrix, ROC Curve & Feature Importance  
- **Training Tools:**  
  - Watsonx.ai Studio notebooks  
  - Hyperparameter tuning via `GridSearchCV`  
  - 5‑fold cross‑validation

---

## 🌐 Deployment Pipeline

The model is served via **IBM Watsonx.ai Runtime**, providing a REST API for real-time inference.

**Steps:**
1. Export trained model (`.pkl`) to IBM Cloud Object Storage  
2. Configure and deploy model in Watsonx.ai Runtime  
3. Expose a **REST API endpoint**  
4. API accepts JSON sensor readings and returns:  
   - `predicted_class`  
   - `confidence` score

---

## 📊 Results & Insights

- Torque and temperature emerged as the strongest predictors.  
- Model achieved high precision and recall across failure classes.  
- Visualizations (ROC curve, confusion matrix) confirm robust performance.  
- Real‑time API responds within milliseconds, ready for live integration.

---

## 🔮 Future Enhancements

- Leverage LSTM or Transformer architectures for time‑series data  
- Estimate Remaining Useful Life (RUL) of equipment  
- Integrate with IoT platforms for streaming sensor data  
- Deploy on edge devices for low‑latency inference  
- Automate maintenance alerts via ERP or messaging systems

---

## 📚 References

- Kaggle Predictive Maintenance Dataset  
- IBM Watsonx.ai Documentation  
- Scikit‑learn Documentation  
- Academic research on predictive maintenance and prognostics

---

## 👨‍💻 Author

**Tushar Kapoor**  
B.Tech – Computer Science & Engineering (AI & ML)  
 Internship Project – 2025  
📧 tusharkapoor052@gmail.com  
🌐 (https://github.com/Tusharkapoor-oop)
