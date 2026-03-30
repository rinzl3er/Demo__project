# Demo__project
### Software and tools requirement

1. [Git](https://github.com)
2. [Visual Studio Code](https://code.visualstudio.com/)

# 🎓 Student Performance Prediction (ML Project)

## 📌 Overview

This project aims to predict student academic performance based on various demographic and educational factors such as gender, parental education, lunch type, and test preparation course.

The project follows a **modular machine learning pipeline architecture**, including data ingestion, transformation, model training, and evaluation.

---

## 🚀 Project Objectives

* Analyze student performance dataset
* Build a robust ML pipeline
* Perform feature engineering and preprocessing
* Train and evaluate regression models
* Deploy a reusable and scalable project structure

---

## 🧠 Problem Statement

Given student attributes, predict the **math score** of a student.

---

## 🗂️ Project Structure

```
Student-Performance-Prediction/
│
├── artifacts/                # Generated files (datasets, models, preprocessor)
│   ├── data.csv
│   ├── train.csv
│   ├── test.csv
│   ├── preprocessor.pkl
│   └── model.pkl
│
├── notebooks/               # Jupyter notebooks (EDA & experiments)
│   ├── data/
│   │    └── stud.csv
│   ├── 1. EDA STUDENT PERFORMANCE.ipynb
│   └── 2. MODEL TRAINING.ipynb
│
├── src/
│   ├── components/
│   │    ├── data_ingestion.py
│   │    ├── data_transformation.py
│   │    └── model_trainer.py
│   │
│   ├── pipeline/
│   │    └── training_pipeline.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── venv/                    # Virtual environment
├── requirements.txt
├── setup.py
└── README.md
```

---

## ⚙️ Tech Stack

* **Python 3.10**
* **Pandas, NumPy**
* **Scikit-learn**
* **Matplotlib, Seaborn**
* **Pickle (Model Serialization)**

---

## 🔄 ML Pipeline Workflow

### 1. Data Ingestion

* Reads dataset from source
* Splits into train & test datasets
* Saves raw and processed files

### 2. Data Transformation

* Handles missing values
* Applies encoding to categorical features
* Scales numerical features
* Saves preprocessing pipeline (`preprocessor.pkl`)

### 3. Model Training

* Trains regression models
* Evaluates performance
* Saves best model (`model.pkl`)

---

## 📊 Features Used

### Numerical Features

* writing_score
* reading_score

### Categorical Features

* gender
* race_ethnicity
* parental_level_of_education
* lunch
* test_preparation_course

---

## 🧪 How to Run the Project

### Step 1: Clone the repository

```bash
git clone <your-repo-link>
cd Student-Performance-Prediction
```

### Step 2: Create & activate virtual environment

```bash
python -m venv venv
venv\Scripts\activate   # Windows
```

### Step 3: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the pipeline

```bash
python -m src.components.data_ingestion
```

---

## 📈 Sample Output

After running the pipeline, the following files are generated:

```
artifacts/
 ├── data.csv
 ├── train.csv
 ├── test.csv
 ├── preprocessor.pkl
 └── model.pkl
```

---

## 📌 Key Highlights

* Modular and scalable ML architecture
* Production-level folder structure
* Custom logging and exception handling
* Reusable preprocessing pipeline
* Clean separation of concerns

---

## ⚠️ Common Issues & Fixes

| Issue                | Solution                         |
| -------------------- | -------------------------------- |
| File not found error | Ensure correct working directory |
| Kernel crash         | Install `ipykernel` in venv      |
| Model not saving     | Check artifacts path             |
| Import errors        | Run using `python -m`            |

---

## 📚 Future Improvements

* Add Flask/FastAPI deployment
* Integrate CI/CD pipeline
* Add model monitoring
* Hyperparameter tuning
* Docker containerization

---

## 👨‍💻 Author

**Harsh Trivedi**

---

## ⭐ Acknowledgements

* Scikit-learn documentation
* Kaggle dataset inspiration
* ML pipeline best practices

---

## 📬 Contact

Fe