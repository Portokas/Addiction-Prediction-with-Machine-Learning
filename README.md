# Addiction-Prediction-with-Machine-Learning

Paper Title: From Legal to Illicit Substances: Unveiling Personality Influences with Machine Learning

This project investigates the role of personality and demographic traits in predicting the transition from legal to illicit drug use, with a primary focus on nicotine as the “gateway” substance. Using machine learning techniques and psychological profiling, we aim to enhance addiction risk prediction models and provide more effective tools for behavioral analysis and tailored rehabilitation.

🧠 Overview

Drug addiction is a multifaceted societal issue often rooted in psychological and demographic factors. Our study:
	•	Applies supervised Machine Learning Algorithms (AdaBoost and SVM)
	•	Utilizes the Five Factor Model (FFM) of personality
	•	Predicts transitions from nicotine (legal) to illicit drug use
	•	Investigates demographic influences, with emphasis on education level

📊 Dataset
 Source: UCI Machine Learning Repository (Drug Consumption - Quantified)
 Size: 1,885 participants
	•	Features:
	•	Personality traits (NEO-FFI-R): Neuroticism, Extraversion, Openness, Agreeableness, Conscientiousness
	•	Impulsiveness & Sensation Seeking (SS)
	•	Demographics: Age, Gender, Education Level, Ethnicity, Country
	•	Drug use history for 18 substances (legal & illicit)

⚙️ Methodology
	1.	Data Preprocessing:
	•	Categorical encoding
	•	Binary classification of users (User / Non-User)
	2.	Experiment 1:
	•	Goal: Predict if a nicotine user is likely to transition to illicit substances
	•	Models: AdaBoost, SVM
	•	Metrics: Accuracy, Precision, Recall, F1-Score, AUC
	3.	Experiment 2:
	•	Goal: Correlate personality traits & education level with transition risk
	•	Separate analysis for nicotine users and non-nicotine users
	•	Target outcome: illicit drug use likelihood


## License

The source code in this repository is licensed under the MIT License (see the LICENSE file for details).

⚠️ Note: The accompanying research paper is **not** covered by this license. Please refer to the publisher's terms for usage or citation information.
