🧠 NeuroSense – Real-Time Cognitive Load Detection System

NeuroSense is an AI-powered system that detects a person’s cognitive load (mental effort) in real time by analyzing facial expressions via webcam and simulated EEG signals. This project addresses the growing issue of digital fatigue in education and remote work by enabling systems to respond to a user’s mental state non-invasively.

🧩 What Problem We Solved
In today’s screen-heavy world, prolonged digital interaction can cause mental overload, reducing productivity and well-being. Existing solutions are often:

Intrusive (require EEG headsets)

Expensive

Not real-time

Single-modality

We solved this by combining accessible webcam data with public EEG datasets to detect mental load in real time — without needing physical EEG equipment.
************************
💡 What We Built
NeuroSense is a hybrid deep learning system that:

Uses a webcam for facial expression tracking

Uses DEAP and SEED datasets to simulate EEG signals

Processes facial data with a CNN

Processes EEG time-series data with an LSTM

Combines both via a fusion model

Classifies user mental load as Low, Medium, or High in real time
**********************
🔬 How We Did It
1. Facial Expression Recognition

Input: Webcam video stream

Processing: Facial landmarks extracted using OpenCV

Classification: CNN model to estimate mental effort level

2. EEG Signal Analysis

Input: Public datasets (DEAP and SEED)

Processing: Signal normalization and segmentation

Classification: LSTM model to predict load from temporal EEG patterns

3. Fusion Layer

Combines CNN and LSTM predictions

Applies a weighted decision rule to determine final output

4. Output

Final classification: Low / Medium / High

Can be used for alerts, adaptive UI, or data logging
**********************
🛠️ Tools & Technologies
Languages: Python

Libraries: TensorFlow, Keras, OpenCV, NumPy, Matplotlib

Models: CNN (for facial data), LSTM (for EEG)

Datasets:

DEAP Dataset

SEED Dataset
**********************
📈 Visual Outputs
Accuracy comparison (CNN vs LSTM vs Fusion)

Line graph of cognitive load over time

Stacked bar chart (participant-wise load levels)

Confusion matrix for performance evaluation

All visuals are available in the /visuals folder.
**********************
📁 Project Structure

NeuroSense/
├── webcam_module/       # Facial detection code
├── models/              # CNN & LSTM models
├── fusion/              # Fusion logic
├── data/                # EEG sample data
├── visuals/             # Graphs and charts
├── main.py              # Main script to run the system
├── requirements.txt     # Dependencies
└── README.md            # Project documentation

**********************
🎯 Applications
Education: Monitor student attention in online classes

Mental health: Detect fatigue, stress, or overload

Productivity: Suggest breaks or content changes based on user state

Research: Prototype for brain-computer interface systems
**********************
📚 References
Koelstra et al. (2012). DEAP Dataset: Emotion Analysis Using Physiological Signals

Zheng & Lu (2015). EEG-Based Emotion Classification Using Deep Learning

Zhang et al. (2017). Multimodal Emotion Recognition Using EEG and Eye Tracking

LeCun et al. (2015). Deep Learning. Nature

OpenCV Documentation – https://opencv.org

Keras & TensorFlow – https://keras.io / https://www.tensorflow.org
**********************
👨‍💻 Authors
Shahbaz Malik | Shawn Lasrado | Kritik Mahesh
**********************
Presented at the 10th AEIT International Student Research Colloquium (2025)
Guided by Dr. Sundus Zehra, MAHE Dubai
