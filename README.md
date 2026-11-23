# DriveDecision AI 
### Explainable Vehicle Purchase Recommendation Engine

DriveDecision AI is a Machine Learning project that evaluates vehicle configurations using multiple vehicle-related attributes and predicts an overall evaluation category.

The project combines classification algorithms, model evaluation, explainable AI techniques, interactive predictions, and SQL-based data analysis to demonstrate how data science can support structured vehicle evaluation.

---

## 🎯 Project Objective

The objective of DriveDecision AI is to build an intelligent classification system that evaluates vehicle configurations based on:

- Purchase price
- Maintenance cost
- Number of doors
- Passenger capacity
- Luggage boot size
- Safety level

Using these attributes, the model predicts whether a vehicle configuration is:

- **Unacceptable**
- **Acceptable**
- **Good**
- **Very Good**

---

## 💡 Key Features

- **Automated Data Collection:** Downloads and processes the UCI Car Evaluation dataset.
- **Exploratory Data Analysis:** Examines feature distributions, class balance, and relationships between vehicle attributes.
- **Data Preprocessing:** Handles categorical variables using encoding and preprocessing pipelines.
- **Machine Learning Model Comparison:** Compares multiple classification algorithms.
- **Model Evaluation:** Uses accuracy, precision, recall, F1-score, cross-validation, and confusion matrices.
- **Explainable AI:** Uses feature importance, decision-tree analysis, and permutation importance to understand model behaviour.
- **Interactive Predictions:** Allows users to enter vehicle attributes and receive a predicted evaluation.
- **SQL Analytics:** Stores vehicle evaluation data in SQLite and performs analytical queries.
- **Automated Reports:** Generates evaluation reports, visualizations, and model outputs.

---

## 📊 Dataset

**Dataset:** UCI Car Evaluation Dataset

**Source:** https://archive.ics.uci.edu/dataset/19/car+evaluation

The dataset contains vehicle evaluation records with six input attributes and one target variable.

| Feature | Description |
|---|---|
| buying | Buying price |
| maint | Maintenance cost |
| doors | Number of doors |
| persons | Passenger capacity |
| lug_boot | Luggage boot size |
| safety | Safety level |
| class | Evaluation category (target) |

The original dataset contains 1,728 records.

---

## 🤖 Machine Learning Algorithms

The project compares the following models:

1. Dummy Classifier — baseline model
2. Decision Tree Classifier
3. Random Forest Classifier
4. Logistic Regression

The models are evaluated using a stratified train-test split and cross-validation.

### Evaluation Metrics

- Accuracy
- Macro Precision
- Macro Recall
- Macro F1-Score
- Weighted F1-Score
- Confusion Matrix
- Classification Report

---

## 🔍 Explainability

DriveDecision AI incorporates explainability techniques to make model behaviour easier to understand.

- Decision Tree feature importance
- Permutation feature importance
- Decision Tree rule extraction

These techniques help identify which input attributes contribute to the model's predictions.

---

## 🛠️ Technology Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Model Explainability | Permutation Importance, Decision Trees |
| Database | SQLite |
| Development Environment | Google Colab |
| Model Storage | Joblib |

---

## 📁 Project Structure

```text
DriveDecision-AI/
│
├── data/
│
├── models/
│   └── vehicle_classifier.pkl
│
├── outputs/
│   ├── reports/
│   └── visualizations/
│
├── README.md
├── requirements.txt
└── .gitignore
```

*Generated files and additional reports may vary depending on the completed execution.*

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/DriveDecision-AI.git
```

### 2. Navigate to the Project

```bash
cd DriveDecision-AI
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Project

Open the project notebook in Google Colab or Jupyter Notebook and execute the cells in sequence.

The project downloads the dataset directly from its source, so a separate manual dataset download is not required.

---

## 📈 Expected Outputs

Depending on the execution, the project generates:

- Dataset analysis and visualizations
- Model comparison results
- Classification reports
- Confusion matrices
- Feature importance analysis
- Permutation importance results
- Interactive vehicle evaluation predictions
- SQLite analytical query results
- Saved trained model

---

## ⚠️ Important Limitations

- The project uses the historical UCI Car Evaluation dataset, not a modern database of commercially available vehicles.
- Its evaluation categories are dataset labels, not official crash-test ratings or verified vehicle safety certifications.
- Predictions should not be treated as professional automotive purchasing or safety advice.
- The dataset is relatively small and uses categorical attributes, so the model is a research and portfolio prototype rather than a production vehicle recommendation platform.

---

## 🔮 Future Improvements

- Integrate real-world vehicle specifications and pricing data.
- Add vehicle brand, model, fuel type, and mileage information.
- Develop an interactive Streamlit dashboard.
- Add personalized recommendations based on user preferences.
- Expand the dataset with verified modern automotive information.
- Deploy the model through a REST API.

---

##  Author

**Aditya Dhage**

Data Science & AI Enthusiast

---

## 📜 License

This project is intended for educational and portfolio purposes. Check the dataset's terms of use before redistributing the original data.

---

**DriveDecision AI — Turning Vehicle Attributes into Data-Driven Evaluations.**
