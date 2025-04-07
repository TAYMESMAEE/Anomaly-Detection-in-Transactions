# Transaction Anomaly Detection System

![Anomaly Detection Demo](assets/anomaly_demo.gif)

## Overview
Machine learning system for detecting fraudulent transactions using Isolation Forest algorithm. Identifies unusual patterns in:
- Transaction amounts
- Spending frequency
- Historical averages

## Features
- Real-time anomaly scoring
- Confidence level estimation
- Batch processing support
- Model versioning

## Installation
cd transaction-anomaly-detection
pip install -r requirements.txt

Usage
python
Copy
from src.detect_anomalies import AnomalyDetector

detector = AnomalyDetector()
transaction = {
    'Transaction_Amount': 2500.00,
    'Average_Transaction_Amount': 150.00,
    'Frequency_of_Transactions': 30.0
}
result = detector.detect(transaction)
Project Structure
Copy
├── data/              # Raw and processed datasets
├── models/            # Serialized ML models
├── notebooks/         # Exploratory analysis
├── src/               # Python source code
├── tests/             # Unit tests
├── README.md          # Project documentation
└── requirements.txt   # Dependencies
