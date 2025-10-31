📱 Single-Device Multimodal Solution for Predicting Sleep Efficiency & Next-Day Mood

This project builds a single-device, real-world sleep analytics and mood prediction system using only smartphone-based behavioral signals. We detect drops in sleep efficiency before they happen and study their link to next-day mood — enabling proactive health awareness and mental-wellbeing support.

This is likely the first work to predict sudden drops in sleep efficiency (sleep anomalies) using only smartphone multimodal data. 

🎯 Objective

Predict night-to-night sleep efficiency

Detect early signs of poor sleep

Understand how sleep disruptions relate to next-day mood

Build a low-cost, real-world monitoring solution using only mobile-device signals

🧠 Motivation

Sleep efficiency strongly influences mental health, mood, cognitive performance, and physical well-being

Early detection of sleep issues helps individuals adjust behavior & lifestyle

Unlike wearables-only solutions, this method uses multimodal smartphone features, making it more accessible, scalable, and practical

📊 Dataset — GLOBEM Dataset (INS Waves 2018–2021)


✅ One-Class SVM — best balance of precision & recall for anomaly detection

📈 Key Results

Successfully detects unexpected drops in sleep efficiency

Captures behavioral patterns before poor sleep events

Sleep drop strongly correlates with next-day mood score (PHQ)

“PHQ > 2 indicates poor mental health… Statistical significance confirmed.” 


🛠️ Tools & Technologies

Python

Pandas, NumPy

Scikit-learn

LSTM & Autoencoder models (PyTorch / TensorFlow)

Statistical testing & PCA for feature space visualization


📝 Summary

This project introduced a smartphone-only, multimodal sleep health framework that:

Predicts sleep efficiency drops

Detects anomalies in advance

Links sleep pattern disruptions to mental health

Achieves competitive results compared to SOTA anomaly detection benchmarks

A low-cost, scalable early-warning system for digital mental health.
