# 🍃 Mango-Leaf-Detection

This is a simple **Streamlit** web app for detecting mango leaf diseases using an ensemble of feature extractors (**ConvNeXtLarge**, **MobileNetV3Large**) and a **Random Forest Classifier**.

🔍 The app predicts the type of disease on an uploaded leaf image and displays the prediction with its probability.

---

## 📂 **Project Structure**

.
├── main.py # Streamlit app main script
├── app.py # (Optional) Additional app script
├── dashboard.py # (Optional) Dashboard or additional visualization
├── rf_model.pkl # Pre-trained Random Forest model
├── .gitignore # Ignore large model files (.h5)
├── README.md # Project description

markdown
Salin
Edit

> ⚡ **Note:**  
> - The feature extractors (`.h5` files) are large and are not tracked by Git.  
> - If needed, you can download them separately and place them in the project folder.

---

## 🧩 **How It Works**

- The app uses pre-trained **ConvNeXtLarge** and **MobileNetV3Large** as feature extractors on a resized input image (224x224).
- Features from both extractors are concatenated and passed into a **Random Forest** model (`rf_model.pkl`).
- Class prediction index is mapped to a disease label using an inline Python dictionary (`class_labels`) inside `main.py`.  
  👉 This means **no `labels.txt`** is needed — all labels are defined directly in the script for simplicity and maintainability.
## 👥 Collaborators

**Project Leader:**  
- [Davina Azalia Tara](https://github.com/Davinaazalia)  
  Praktikum: Feature Extraction (ConvNeXt), Random Forest Classification, Integration into Streamlit  
  Report: Results and Discussion

**Project Supervisor:**  
- [Fadhlu Ibnu ‘Abbad](https://github.com/fadhluibnu) (Project Advisor)

**Team Members:**  
- [Muhammad Rizky Albani](https://github.com/rzkyalbani)  
  Praktikum: SVM Classification (initial test, not used)  
  Report: Introduction

- [Innayatul Laili Husnaini](https://github.com/innayatullaili)  
  Praktikum: Concatenation ConvNeXt  
  Report: Problem Formulation, Method (Tools Used) — **also serves as Practicum Report Coordinator**

- [Intan Permata Sari Fauziah](https://github.com/Intan-psf)  
  Praktikum: Concatenation MobileNetV3 and Concatenation ConvNeXt + MobileNetV3  
  Report: Method (Data Sources, Data Splitting, Feature Extraction, Model Evaluation)

- [Anita Hasna Zahira Safa](https://github.com/anitah25)  
  Praktikum: Preprocessing (Rescale, Normalization, Rotation)  
  Report: Introduction

- [Raihan Muhammad Nafi’](https://github.com/Raihnmn)  
  Praktikum: Preprocessing (Zoom, Horizontal Flip, Vertical Flip)  
  Report: Results and Discussion

- [Nafisa Salsabila](https://github.com/nafisaslsbl)  
  Praktikum: Feature Extraction  
  Report: Method (Data Preprocessing, Random Forest Classification, Model Training, Tools Used)

---



---

