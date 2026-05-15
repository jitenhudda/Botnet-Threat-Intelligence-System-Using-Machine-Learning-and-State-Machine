# Botnet Threat Intelligence System Using Machine Learning and State Machine

## Overview

The Botnet Threat Intelligence System is a hybrid cybersecurity framework designed to detect and analyze malicious network activities using Machine Learning, Risk Scoring, and State Machine-based behavioral analysis.

The system classifies network traffic patterns and identifies potential threats such as botnet communication, distributed denial-of-service (DDoS) attacks, command-and-control (C2) activity, and suspicious traffic anomalies.

This project integrates:
- Machine Learning Classification
- Behavioral State Analysis
- Threat Risk Scoring
- AI-based Threat Explanation
- Interactive Web Interface using Gradio

---

## Features

- Real-time network traffic analysis
- Machine Learning-based threat classification
- Risk score generation
- Stateful botnet behavior detection
- AI-generated threat explanations
- Interactive Gradio dashboard
- Hybrid detection architecture

---

## System Architecture

The project combines three major detection components:

### 1. Machine Learning Layer
A Random Forest classifier is trained on network traffic features to classify malicious and benign traffic patterns.

### 2. Risk Scoring Engine
The system calculates a dynamic threat risk score using:
- Flow duration
- Packet rate
- Throughput
- Forward packet count

### 3. State Machine Engine
Behavioral transitions are monitored through predefined states:

```text
NORMAL → SUSPICIOUS → INFECTED → C2 → ATTACK
```

The state machine improves detection of multi-stage cyber attacks and botnet progression.

---

## Dataset Requirements

The dataset must contain the following columns:

| Column Name | Description |
|-------------|-------------|
| Flow Duration | Duration of network flow |
| Total Fwd Packets | Total forward packets |
| Flow Bytes/s | Bytes transferred per second |
| Flow Packets/s | Packets transferred per second |
| Label | Traffic classification label |

---

## Feature Engineering

Additional intelligent features are generated to improve detection performance:

```python
Bytes_per_Packet
Packets_per_Duration
Burst_Intensity
PPS_Log
BPS_Log
```

These features help identify abnormal traffic behavior patterns more effectively.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Gradio

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/botnet-threat-intelligence-system.git

cd botnet-threat-intelligence-system
```

### Install Dependencies

```bash
pip install gradio pandas scikit-learn numpy
```

---

## Running the Project

Execute the application using:

```bash
python app.py
```

After execution, Gradio will generate a local URL to access the web interface.

---

## Threat Detection Logic

The system identifies suspicious activities using behavioral indicators:

| Condition | Possible Threat |
|------------|----------------|
| High packets per second | DDoS activity |
| High bytes per second | Data exfiltration |
| Long duration with low packets | Command-and-Control communication |
| High packet volume with low rate | Stealth transfer activity |

---

## User Interface

The Gradio-based dashboard allows users to:
- Input network traffic parameters
- Analyze traffic behavior in real time
- View machine learning predictions
- Monitor risk scores
- Read AI-generated threat explanations

---

## Sample Output

```text
Threat Status: ATTACK

Risk Score: 84.7%

Machine Learning Prediction:
Botnet Traffic

Confidence:
97.3%

AI Threat Analysis:
- Extremely high packet rate detected
- Traffic flooding behavior consistent with DDoS attacks
- Possible command-and-control communication identified
```

---

## Applications

This project can be applied in:
- Intrusion Detection Systems (IDS)
- Botnet Detection Systems
- Cyber Threat Intelligence Platforms
- Academic Research
- Network Security Monitoring
- Security Analytics Solutions

---

## Future Enhancements

Future improvements may include:
- Deep Learning integration
- Real-time packet sniffing
- SIEM integration
- Cloud deployment
- Threat visualization dashboards
- Live network monitoring

---

## Author

Jiten Hudda

---

## Contribution

Contributions are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push the branch
5. Open a pull request

---

## Acknowledgment

This project was developed for educational and research purposes in the field of cybersecurity and machine learning.
