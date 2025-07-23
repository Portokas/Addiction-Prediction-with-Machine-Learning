
# Personality-Based Drug Use Prediction with Machine Learning

This project explores how personality traits (NEO-FFI-R), in combination with demographic features, can be used to predict the transition from legal substances (like nicotine) to illicit drug use using machine learning techniques. The study uses the publicly available "Drug Consumption" dataset and focuses on supervised learning classification, correlation analysis, and ROC evaluation.

## 🧠 Dataset

- **Source**: UCI Machine Learning Repository  
- **Link**: https://archive.ics.uci.edu/dataset/373/drug+consumption+quantified
- **Format**: CSV (`drug_consumption.data`)
- **Size**: 1885 participants
- **Features**:
  - 5 personality traits (NEO-FFI-R): Neuroticism, Extraversion, Openness, Agreeableness, Conscientiousness  
  - Impulsivity, Sensation Seeking  
  - Demographics: Age, Gender, Education, Country, Ethnicity  
  - Use of 18 substances (legal + illegal)

## 📂 Project Structure

```
project/
│
├── data/
│   └── drug_consumption.data
├── src/
│   ├── preprocess.py
│   ├── experiment1_classification.py
│   ├── experiment2_correlations.py
│   └── utils.py
├── figures/
│   └── roc_curve.png
├── results/
│   └── confusion_matrices/
│       ├── adaboost.png
│       └── svm.png
├── requirements.txt
└── README.md
```

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/Portokas/Addiction-Prediction-with-Machine-Learning.git
cd Addiction-Prediction-with-Machine-Learning
```

2. (Optional) Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

## ⚙️ How to Reproduce

1. Download the dataset from the UCI link above.
2. Place `drug_consumption.data` into the `/data` folder.

Then run:

```bash
python src/preprocess.py
python src/experiment1_classification.py
python src/experiment2_correlations.py
```

## 📊 Output

- Accuracy, Precision, Recall, F1-score
- ROC curve comparison between AdaBoost & SVM
- Correlation heatmaps for education vs drug use
- Confusion matrices

## 📚 Citation

> A. Portokallidis, “From Legal to Illicit Substances: Personality-Based Drug Use Prediction with Machine Learning”, 2025.

## 🙋 Author

- Athanasios Portokallidis  
- th20109@edu.hmu.gr

## 📄 License

This project is licensed under the MIT License.
