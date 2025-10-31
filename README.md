📱 Single-Device Multimodal Solution for Predicting Sleep Efficiency & Next-Day Mood

This project builds a single-device, real-world sleep analytics and mood prediction system using only smartphone-based behavioral signals. We detect drops in sleep efficiency before they happen and study their link to next-day mood — enabling proactive health awareness and mental-wellbeing support.

This is likely the first work to predict sudden drops in sleep efficiency (sleep anomalies) using only smartphone multimodal data. 

CSE 570 Final Presentation (1)

🎯 Objective

Predict night-to-night sleep efficiency

Detect early signs of poor sleep

Understand how sleep disruptions relate to next-day mood

Build a low-cost, real-world monitoring solution using only mobile-device signals

🧠 Motivation

Sleep efficiency strongly influences mental health, mood, cognitive performance, and physical well-being

Early detection of sleep issues helps individuals adjust behavior & lifestyle

Unlike wearables-only solutions, this method uses multimodal smartphone features, making it more accessible, scalable, and practical

“Sleep efficiency is a critical indicator of overall health… early detection helps adapt routines, environment, and behaviors.” 

CSE 570 Final Presentation (1)

📊 Dataset — GLOBEM Dataset (INS Waves 2018–2021)
Wave	Year	Participants Used
INS-W1	2018	50
INS-W2	2019	50
INS-W3	2020	50
INS-W4	2021	50
Data Sources

Smartphone screen usage

Daily steps

Location-linked events

Sleep summary information

Preprocessing Steps

Removed rows with >90% null values

Median imputation for other missing values

Daily-level feature extraction

Sleep efficiency binning

“Took 50 participants from each year… dropped 90% null rows and imputed others with median value.” 

CSE 570 Final Presentation (1)

🏷️ Sleep Efficiency Binning & Anomaly Labeling
Sleep Efficiency (%)	Label
45–70	0
70–85	1
85–90	2
90–100	3

>85% = good sleep

If current bin < previous bin ⇒ sleep anomaly (1)

Only 0.4% days labeled as anomalies — real-world rare event.

“Sleep efficiency above 85% is considered good… anomaly % is 0.4%.” 

CSE 570 Final Presentation (1)

🧮 Selected Features
Behavioral Features

Minimum daily steps

First unlock time after midnight

Screen usage behavior

Sleep Features

Sleep efficiency

First bedtime

Last bedtime

Previous-day sleep behavior (derived)

🧪 Models Used
Category	Models
Unsupervised	One-Class SVM, Isolation Forest
Supervised	Random Forest
Ensemble	Majority Voting, Soft Voting
Deep Learning	LSTM, Autoencoder
Best Model

✅ One-Class SVM — best balance of precision & recall for anomaly detection

📈 Key Results

Successfully detects unexpected drops in sleep efficiency

Captures behavioral patterns before poor sleep events

Sleep drop strongly correlates with next-day mood score (PHQ)

“PHQ > 2 indicates poor mental health… Statistical significance confirmed.” 

CSE 570 Final Presentation (1)

🛠️ Tools & Technologies

Python

Pandas, NumPy

Scikit-learn

LSTM & Autoencoder models (PyTorch / TensorFlow)

Statistical testing & PCA for feature space visualization

🔮 Future Work

Real-time anomaly detection system

Personalized recommendations

User studies to validate behavior-based feedback

Improve precision via filtering and hybrid models

👥 Contributors
Name	Contribution
Jamalia Jisha	Data processing, problem formulation, modeling
Adiba Shaira	Related work, feature extraction, modeling, analysis
📝 Summary

This project introduced a smartphone-only, multimodal sleep health framework that:

Predicts sleep efficiency drops

Detects anomalies in advance

Links sleep pattern disruptions to mental health

Achieves competitive results compared to SOTA anomaly detection benchmarks

A low-cost, scalable early-warning system for digital mental health.
