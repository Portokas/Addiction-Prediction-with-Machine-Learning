# Addiction-Prediction-with-Machine-Learning

Paper Title: From Legal to Illicit Substances: Unveiling Personality Influences with Machine Learning

This project explores how personality and demographic traits influence the transition from legal to illicit drug use, focusing primarily on nicotine as a gateway substance. By leveraging supervised machine learning algorithms and psychological profiling based on the Five Factor Model (FFM), the study aims to predict addiction risk and assist in faster, more personalized rehabilitation approaches.

The dataset used is the “Drug Consumption (Quantified)” dataset from the UCI Machine Learning Repository, which contains 1,885 participants with no missing values. Each participant is described by 12 features including personality traits (neuroticism, extraversion, openness, agreeableness, conscientiousness), impulsiveness, sensation seeking, age, gender, education level, country of residence, and ethnicity. In addition, participants reported their usage of 18 substances, both legal and illicit.

The methodology consists of two main experiments. In the first, we applied and compared the performance of two supervised machine learning algorithms, AdaBoost and Support Vector Machine (SVM), to predict whether nicotine users are likely to transition to illicit drug use. Data were preprocessed and split into training and testing subsets, and models were evaluated using accuracy, precision, recall, F1-score, and area under the ROC curve (AUC). The results showed that both classifiers performed well, with AdaBoost slightly outperforming SVM. Specifically, AdaBoost achieved an accuracy of 74% and an AUC of 0.84, while SVM reached 75% accuracy and an AUC of 0.83.

In the second experiment, the dataset was divided into nicotine users and non-users in order to examine how personality traits correlate with illicit drug use based on a person’s education level. Among nicotine users, 46.90% had transitioned to illicit drug use, whereas 15.65% of non-nicotine users had used illegal substances directly. Correlation analysis revealed that for nicotine users, openness to experience (Oscore) is the strongest personality trait linked to illicit drug use, especially when factoring in education. For non-nicotine users, impulsiveness and sensation seeking (SS) were more dominant predictors.

The findings suggest that psychologists and professionals can assess addiction risk by focusing on a single domain of the NEO-FFI-R personality model, specifically the one most correlated with the individual’s legal drug use behavior. By combining this domain with the person’s education level and history of nicotine use, practitioners can predict the likelihood of transitioning to illicit drug use with fewer resources and greater speed.

This study contributes to the existing literature by proposing a simplified, targeted method for addiction risk analysis using machine learning. Future work may include extending this methodology to other legal substances beyond nicotine and exploring additional correlations between personality traits and social factors in substance use behavior.

## License

The source code in this repository is licensed under the MIT License (see the LICENSE file for details).

⚠️ Note: The accompanying research paper is **not** covered by this license. Please refer to the publisher's terms for usage or citation information.
