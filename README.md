# 🧠 Multimodal Parkinson’s Disease Detection System

## 📌 Overview

This project presents a machine learning-based system for early detection of Parkinson’s disease using both **voice signal features** and **tremor (accelerometer) data**.

The system leverages multimodal data to improve detection accuracy and provide a more reliable assessment compared to single-source methods.

---

## 🎯 Objectives

* Detect Parkinson’s disease using **voice-based biomarkers**
* Analyze tremor patterns using **accelerometer-derived features**
* Combine both modalities for improved prediction accuracy
* Provide a **non-invasive, early-stage screening tool**

---

## 🧩 Features

* 🎤 Voice-based detection using acoustic features (Jitter, Shimmer, HNR, etc.)
* 📈 Tremor-based detection using statistical and frequency-domain features
* 🤖 Machine Learning models (Random Forest, SVM, Logistic Regression)
* 📊 Model comparison and accuracy evaluation
* 🔍 Feature importance analysis
* ⚡ Real-time prediction interface (UI)

---

## 📂 Datasets Used

### 1. Voice Dataset

Includes features such as:

* Jitter, Shimmer, HNR
* RPDE, DFA, PPE
* UPDRS scores (severity indicators)

### 2. Tremor Dataset

Derived from accelerometer signals:

* Time-domain features (mean, variance, RMS, peaks)
* Frequency-domain features (FFT, dominant frequency, entropy)
* Complexity measures (Sample Entropy, DFA)
* Tremor labels:

  * Rest tremor
  * Postural tremor
  * Kinetic tremor

---

## 🛠️ Technologies Used

* Python
* Scikit-learn
* Pandas, NumPy
* Google Colab / Jupyter Notebook
* Flask / Streamlit (for UI)

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Handling missing values
* Feature selection
* Data normalization (StandardScaler)

### 2. Model Training

* Train-test split
* Multiple models trained:

  * Random Forest
  * Support Vector Machine (SVM)
  * Logistic Regression

### 3. Evaluation

* Accuracy score
* Precision & Recall
* Model comparison

### 4. Prediction

* Output includes:

  * Disease detection (Yes/No)
  * Confidence score
  * Feature contribution (optional)

---

## 🔗 System Architecture

```
Voice Input → Feature Extraction → ML Model → Prediction
Tremor Data → Feature Processing → ML Model → Prediction

                ↓
        Multimodal Fusion
                ↓
        Final Decision Output
```

---

## 🚀 How to Run

### Step 1: Clone the repository

```
git clone <your-repo-link>
cd <project-folder>
```

### Step 2: Install dependencies

```
pip install -r requirements.txt
```

### Step 3: Train the model (optional)

Run the notebook in:

* Google Colab or Jupyter Notebook

### Step 4: Run the application

```
python app.py
```

---

## 📊 Output Example

* Prediction: Parkinson’s Disease Detected
* Confidence: 87%
* Key Features: High Jitter, Low HNR, High Tremor Energy

---

## 🔬 Key Insights

* Voice features can detect Parkinson’s in early stages
* Tremor analysis confirms motor symptoms
* Multimodal approach improves robustness and reliability

---

## ⚠️ Disclaimer

This project is intended for **educational and research purposes only**.
It is not a substitute for professional medical diagnosis.

---

## 🔮 Future Work

* Real-time voice recording integration
* Mobile application deployment
* Integration with wearable sensors
* Deep learning-based feature extraction
* Clinical validation with real patient data

---

## 👨‍💻 Authors

* Your Name

---

## 📜 License

This project is open-source and available under the MIT License.

---
