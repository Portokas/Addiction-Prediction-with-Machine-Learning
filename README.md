
# Personality-Based Drug Use Prediction with Machine Learning

This project explores how personality traits (NEO-FFI-R), in combination with demographic features, can be used to predict the transition from legal substances (like nicotine) to illicit drug use using machine learning techniques. The study uses the publicly available "Drug Consumption" dataset and focuses on supervised learning classification, correlation analysis, and ROC evaluation.

## Dataset

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

## Installation

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

## How to Reproduce

1. Download the dataset from the UCI link above.
2. Place `drug_consumption.data` into the `/data` folder.

Then run:

```bash
python src/preprocess.py
python src/experiment1_classification.py
python src/experiment2_correlations.py
```

## Output

- Accuracy, Precision, Recall, F1-score
- ROC curve comparison between AdaBoost & SVM
- Correlation heatmaps for education vs drug use
- Confusion matrices

## Conclusion

This study demonstrates that personality traits, especially when measured through validated psychometric instruments like the NEO-FFI-R, can serve as meaningful predictors for identifying the likelihood of transitioning from legal to illicit drug use. By applying machine learning techniques such as AdaBoost and SVM, we observed strong classification performance, particularly among nicotine users. These findings highlight the potential for using personality-based models to support early prevention strategies and personalized interventions in substance use research.

## Proper Citation

A. Portokallidis, I. Manolis, K. Karampidis, M. Tampouratzis, and M. Kara, "From Legal to Illicit Substances: Unveiling Personality Influences with Machine Learning," Department of Electrical and Computer Engineering, Hellenic Mediterranean University, Heraklion, Greece, and Interdisciplinary Research Center for Intelligent Secure Systems, King Fahd University of Petroleum and Minerals, Dhahran, Saudi Arabia.

## Author

- Athanasios Portokallidis  
- portokallidesthanases@gmail.com

## License

This project is licensed under the MIT License.
