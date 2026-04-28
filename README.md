# Network Attack Detection System (ML + GUI)

## 🚀 Project Overview

This project presents a Machine Learning-based Intrusion Detection System (IDS) capable of identifying anomalous network behavior in real time. It combines an unsupervised anomaly detection model with an interactive graphical user interface (GUI) to monitor and analyze network traffic patterns.

The system is designed to simulate real-world cybersecurity scenarios where detecting unknown or zero-day attacks is critical. By leveraging machine learning techniques, the model identifies unusual patterns without requiring labeled attack data.

## 🎯 Objective

The main goals of this project are:

- Detect anomalous network behavior using machine learning  
- Build a real-time intrusion detection interface  
- Provide an interactive GUI for monitoring  

Additionally, the project focuses on:

- Understanding unsupervised learning techniques  
- Simulating real-world cybersecurity scenarios  
- Creating a scalable prototype for IDS systems

## 🧠 Core Concept
This project uses the Isolation Forest Algorithm, which is specifically designed for anomaly detection.
Instead of learning normal vs attack patterns explicitly, the model:
Learns the structure of normal data
Identifies anomalies as data points that are “isolated” quickly
This makes it highly effective for:
Unknown attacks
Zero-day threats
Unlabeled datasets

⚙️ Technologies Used
Python
NumPy & Pandas — Data processing
Scikit-learn — Isolation Forest model
Joblib — Model saving/loading
Tkinter — GUI development
Threading & Queue — Real-time simulation

## ✨ Features

- 🔍 Real-time anomaly detection  
- 📊 Live monitoring dashboard  
- 📂 CSV & Excel file support  
- 🤖 Machine learning-based prediction  
- 🎯 Unsupervised learning (no labeled data required)  
- 📈 Dynamic anomaly rate calculation  
- 🎨 Color-coded visualization (Anomaly vs Normal)  

## 🧪 Execution Steps

### Step 1: Install Dependencies

Install required Python libraries:

pip install -r requirements.txt

(Optional for Excel support):
pip install openpyxl

---

### Step 2: Run the Application

Execute the GUI script:

python Network_threat_detector_gui.py

---

### Step 3: Interact with the System

- Click **Start** → Begin live traffic simulation  
- Click **Upload CSV** → Analyze external dataset  
- Click **Stop** → Pause monitoring  
- Click **Clear** → Reset statistics and table  


## 🔄 How It Works

The system follows this pipeline:

1. Data is collected (synthetic or uploaded file)  
2. Features are extracted and preprocessed  
3. Protocol values are encoded into numeric format  
4. Data is passed into the trained Isolation Forest model  
5. Model outputs:
   - 1 → Normal  
   - -1 → Anomaly  
6. Results are displayed in the GUI in real time  

## 🚀 Future Scope

This project can be enhanced by:

- Integrating real-time packet capture using Scapy  
- Using deep learning models (LSTM, Autoencoders)  
- Deploying as a web-based dashboard (Flask/React)  
- Adding alert systems (Email/SMS notifications)  
- Connecting with SIEM tools for enterprise usage  
