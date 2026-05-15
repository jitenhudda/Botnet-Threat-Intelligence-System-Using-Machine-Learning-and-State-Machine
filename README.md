# 🛡️ Botnet Threat Intelligence System Using Machine Learning and State Machine

An AI-powered **Botnet Threat Detection & Intelligence System** that combines **Machine Learning**, **Behavioral State Analysis**, and **Risk Scoring** to detect malicious network activities in real time.

This system analyzes network traffic patterns to identify cyber threats such as:

* Botnet infections
* DDoS attacks
* Command & Control (C2) communication
* Data exfiltration
* Suspicious traffic anomalies

Built using:

* Python
* Scikit-learn
* Pandas
* Gradio

---

# 🚀 Features

✅ Machine Learning based traffic classification
✅ Hybrid threat detection architecture
✅ Stateful botnet behavior analysis
✅ Dynamic risk scoring engine
✅ AI-generated threat explanations
✅ Interactive Gradio dashboard
✅ Real-time network threat analysis

---

# 📌 Project Overview

Traditional intrusion detection systems often fail to detect evolving botnet behavior patterns.
This project introduces a **hybrid cyber threat intelligence framework** that combines:

1. **Machine Learning Classification**
2. **Risk-Based Analysis**
3. **Finite State Machine Detection**

The system continuously evaluates traffic behavior and predicts possible botnet activities.

---

# 🧠 Detection Architecture

## Hybrid Detection System

The framework consists of three major layers:

### 1️⃣ Machine Learning Layer

A `RandomForestClassifier` is trained on network traffic data to classify malicious and benign behavior.

### 2️⃣ Risk Scoring Engine

Calculates threat severity using:

* Packet rate
* Flow duration
* Throughput
* Packet count

### 3️⃣ State Machine Engine

Tracks behavioral progression of network threats.

```text
NORMAL → SUSPICIOUS → INFECTED → C2 → ATTACK
```

---

# 📂 Dataset Requirements

The CSV dataset must contain the following columns:

| Column Name       | Description                    |
| ----------------- | ------------------------------ |
| Flow Duration     | Duration of traffic flow       |
| Total Fwd Packets | Total forward packets          |
| Flow Bytes/s      | Bytes transferred per second   |
| Flow Packets/s    | Packets transferred per second |
| Label             | Traffic label/category         |

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/botnet-threat-intelligence-system.git

cd botnet-threat-intelligence-system
```

---

## 2️⃣ Install Dependencies

```bash
pip install gradio pandas scikit-learn numpy
```

---

# ▶️ Run the Project

```bash
python app.py
```

After running the program, Gradio will generate a local URL.
Open it in your browser to access the dashboard.

---

# 📊 Feature Engineering

The system creates additional intelligent security features:

```python
Bytes_per_Packet
Packets_per_Duration
Burst_Intensity
PPS_Log
BPS_Log
```

These engineered features improve anomaly detection performance.

---

# 🧪 Threat Analysis Logic

## Threat Indicators

| Condition                      | Possible Threat   |
| ------------------------------ | ----------------- |
| Very high PPS                  | DDoS attack       |
| High BPS                       | Data exfiltration |
| Long duration + low packets    | C2 beaconing      |
| Large packet volume + low rate | Stealth transfer  |

---

# 🖥️ User Interface

The Gradio dashboard allows users to:

* Adjust traffic parameters
* Analyze traffic instantly
* View risk scores
* Monitor ML predictions
* Read AI-generated threat explanations

---

# 📸 Sample Output

```text
🚨 Threat Status: ATTACK
🔥 Risk Score: 84.7%

Machine Learning Prediction:
Botnet Traffic

Confidence:
97.3%

AI Threat Analysis:
• Extremely high packet rate detected
• Traffic flooding behavior consistent with DDoS attacks
• Possible command & control communication identified
```

---

# 🏗️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Gradio

---

# 🔒 Security Applications

This project can be used for:

* Botnet Detection Systems
* Intrusion Detection Systems (IDS)
* Cybersecurity Research
* Threat Intelligence Platforms
* Academic Projects
* Network Monitoring Solutions

---

# 📈 Future Enhancements

* Deep Learning Integration
* Live Packet Sniffing
* Real-Time Traffic Capture
* SIEM Integration
* Cloud Deployment
* Threat Visualization Dashboard

---

# 🤝 Contributing

Contributions are welcome.

### Steps:

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

# 📜 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Jiten Hudda**

* Cybersecurity Enthusiast
* Machine Learning Developer
* Network Security Researcher

---

# ⭐ Support

If you found this project useful:

⭐ Star the repository
🍴 Fork the project
🛡️ Share with cybersecurity enthusiasts
