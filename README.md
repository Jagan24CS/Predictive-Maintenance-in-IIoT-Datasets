# 🔧 Predictive Maintenance in IoT Datasets

A machine learning-based Predictive Maintenance (PdM) solution developed in an Industrial IoT (IIoT) environment. This project aims to detect early signs of failure using synthetic sensor data, simulating real-world machine behaviors.

---

## 📂 Dataset Creation

The dataset used in this project was **custom-built from scratch** rather than using any existing public datasets. This approach was essential due to the following reasons:

- 🔍 **Lack of publicly available datasets:** No general-purpose datasets were found that suited the requirements of an IIoT-based predictive maintenance system.
- 🔐 **Domain-specific limitations:** Most available datasets are highly tailored to specific industrial setups, reducing their applicability in broader use cases.
- 🎛️ **Custom control over data:** Creating the dataset from scratch allowed:
  - Simulation of varied sensor behaviors (temperature, pressure, vibration, etc.)
  - Injection of realistic operational and degraded conditions
  - Controlled introduction of faults and anomalies for model training

Sensor readings were generated using Python-based simulations over a period, with clear labeling of normal and faulty operations.

---

## 🧠 Model Training Methodology

The machine learning model was trained using the following methodology:

### 🧹 Preprocessing
- **Normalization** of sensor data
- **Time-windowing** for sequential learning

### 📈 Algorithms
- Multiple algorithms were evaluated.
- Focused primarily on:
  - **Random Forest**
  - **XGBoost**
  
These were selected for their strong performance on structured/tabular sensor data.

### 📊 Evaluation Metrics
- Model performance was assessed using:
  - **Accuracy**
  - **Precision**
  - **Recall**

---

## ⚠️ Why is Accuracy Currently Low?

The current model accuracy is limited due to:

- Imperfect simulation of real-world conditions
- **Imbalanced class distribution**
- **Presence of noise** in the generated sensor data

🚧 **Ongoing Work:**
Efforts are underway to improve:
- Dataset realism
- Labeling strategies
- Balance of classes

These enhancements are expected to significantly improve model performance in future iterations.

---

## 📌 Project Goals
- Create a reusable, extensible predictive maintenance pipeline
- Contribute a generalized synthetic PdM dataset for the IoT domain
- Enable real-time failure prediction using low-cost simulation data

---

## 📚 Technologies Used
- Python, NumPy, Pandas
- Scikit-learn, XGBoost
- Matplotlib/Seaborn for visualization
