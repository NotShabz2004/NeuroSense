NeuroSense – Real-Time Cognitive Load Detection System
NeuroSense is an AI-driven system that detects a person’s cognitive load (mental effort) in real time by analyzing facial expressions via webcam and simulated EEG signals from well-known datasets. Our project addresses the growing issue of digital fatigue in education and remote work settings by enabling systems to become responsive to the user’s mental state.

🧩 What Problem We Solved
In today's digital-first world, prolonged screen time can cause mental overload, which affects focus, productivity, and overall well-being. Existing systems either:

Lack real-time responsiveness

Rely on intrusive or expensive EEG hardware

Don't combine multiple indicators of mental state

We built a non-invasive, AI-based solution that can assess mental effort live — using just a webcam and public datasets.

💡 What We Built
NeuroSense is a hybrid machine learning system that:

Takes live facial video from a webcam

Uses EEG signals from public datasets (DEAP & SEED)

Analyzes both data types using deep learning

Fuses the results to detect real-time cognitive load (Low / Medium / High)

It is designed to be:

Real-time

Scalable

Affordable (no need for EEG headgear)

🔬 How We Did It
1. Facial Expression Recognition
Live webcam data captured using OpenCV

Facial landmarks extracted and fed into a Convolutional Neural Network (CNN)

CNN classifies cognitive load based on subtle expression patterns

2. EEG Signal Classification
We used DEAP and SEED datasets to simulate EEG input

Signals were preprocessed (filtered, normalized)

Processed via a Long Short-Term Memory (LSTM) model to capture time-based patterns

3. Fusion Layer
We combined CNN and LSTM outputs using a weighted decision fusion strategy

The final decision represents one of three cognitive load states

4. Output
The system gives a real-time result: Low, Medium, or High load

Can be extended to adjust UI/UX based on user state

🛠️ Tools & Technologies
Languages: Python

Libraries: TensorFlow, Keras, OpenCV, NumPy, Matplotlib

Models: CNN for spatial analysis, LSTM for time-series EEG

Datasets:

DEAP Dataset

SEED Dataset

📈 Visual Outputs
We created graphs to show:

Model accuracy comparison: CNN vs LSTM vs Fusion

Confusion matrix for final predictions

Real-time cognitive load trends (line graphs)

Participant-wise load analysis (bar charts)

(See /visuals folder)

📁 Project Structure
webcam_module/ – Facial expression detection pipeline

models/ – Training and evaluation of CNN & LSTM

fusion/ – Decision strategy combining both outputs

data/ – Preprocessed EEG data (simulated)

visuals/ – All graphs and diagrams

main.py – System entry point for testing and integration

requirements.txt – Python dependencies

🎯 Applications
Online education – Track and adapt to student mental effort

Mental health monitoring – Detect fatigue, burnout, or stress levels

Work-from-home productivity – Systems that know when you're losing focus

Research and BCI – Early-stage brain-computer interaction framework

📚 References
Koelstra et al., DEAP Dataset: Emotion Analysis Using Physiological Signals, IEEE (2012)

Zheng & Lu, EEG-Based Emotion Classification Using Deep Learning, IEEE (2015)

Zhang et al., Multimodal Emotion Recognition with EEG and Eye Tracking (2017)

LeCun et al., Deep Learning, Nature (2015)

OpenCV, TensorFlow, and Keras Official Documentation

👨‍💻 Team
Shahbaz Malik
Shawn Lasrado
Kritik Mahesh

Presented at the 10th AEIT International Student Research Colloquium (2025)
Under the guidance of Dr. Sundus Zehra, MAHE Dubai
