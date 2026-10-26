# AI-Powered Network Intrusion Detection System (NIDS)
### IBM SkillsBuild Cyber Security 2026 | Conducted by BharatCares

**Candidate Name:** Vaishnavi Gondal  
**Program:** IBM SkillsBuild Cyber Security Internship 2026  
**Implementation Partner:** BharatCares  
**Project Domain:** Cyber Threat Intelligence, Network Security & Machine Learning  

---

## 📌 Project Overview
Modern enterprise networks face an unprecedented volume of sophisticated cyber-attacks, ranging from Distributed Denial of Service (DDoS) and automated port scans to remote-to-local privilege escalations. Traditional signature-based Intrusion Detection Systems (IDS) frequently fail to detect zero-day exploits and novel attack variants.

This project implements an **AI-Powered Network Intrusion Detection System (NIDS)** that utilizes supervised machine learning algorithms to inspect packet-level telemetry data in real time. The system classifies incoming network traffic as either benign or malicious and categorizes specific attack vectors (DoS, Probe, R2L, U2R) with high precision, maintaining low False Alarm Rates (FAR) to prevent Security Operations Center (SOC) alert fatigue.

---

## 🚀 Key Features
- **High-Accuracy Attack Detection:** Evaluated across multiple classifiers (Random Forest, Decision Trees, Gradient Boosting, Logistic Regression), achieving **99.2% classification accuracy**.
- **Real-Time Traffic Scoring:** Custom inference pipeline (`inspect_packet_traffic`) capable of parsing network features and issuing immediate incident responses.
- **Dimensionality Reduction & Feature Importance:** Identifies the top network attributes indicative of malicious intent (e.g., connection count, SYN error rate, source-to-destination bytes).
- **Enterprise-Ready Modularity:** Structured for direct integration with SOC dashboards, SIEM tools (Splunk, Elastic SIEM), and live packet capture tools (Scapy/Wireshark).

---

## 📊 Dataset Reference
- **Benchmark Dataset:** [NSL-KDD Network Intrusion Dataset (Kaggle / University of New Brunswick)](https://www.kaggle.com/datasets/hassan06/nslkdd)
- **Secondary Reference:** [CIC-IDS2017 Dataset (Canadian Institute for Cybersecurity)](https://www.unb.ca/cic/datasets/ids-2017.html)
- **Features Analyzed:** 41 distinct network features including basic TCP/IP connection attributes, traffic rates within 2-second windows, and host-based multi-connection statistics.

---

## 🛠️ Technologies & Stack
- **Programming Language:** Python 3.10+
- **Machine Learning & Analytics:** Scikit-Learn, NumPy, Pandas, Joblib
- **Data Visualization:** Matplotlib, Seaborn
- **Development Environment:** Jupyter Notebook (`.ipynb`), VS Code
- **Documentation:** Microsoft Word (`.docx`), Markdown (`.md`)

---

## ⚙️ Installation & Execution Guide

### 1. Clone or Extract the Repository
```bash
git clone https://github.com/VaishnaviGondal/NIDS-IBM-SkillsBuild.git
cd NIDS-IBM-SkillsBuild
```

### 2. Set Up a Virtual Environment (Recommended)
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook VaishnaviGondal_NetworkIntrusionDetection.ipynb
```
Execute cells sequentially to inspect data generation, exploratory analysis, model training, and sample packet inference.

---

## 📈 Evaluation Results Summary

| Model Algorithm | Accuracy | Precision | Recall | F1-Score | Status |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Random Forest (Champion)** | **99.20%** | **99.10%** | **99.30%** | **99.20%** | **Deployed** |
| Gradient Boosting | 98.40% | 98.10% | 98.50% | 98.30% | Alternate |
| Decision Tree | 97.10% | 96.80% | 97.40% | 97.10% | Baseline |
| Logistic Regression | 88.50% | 89.20% | 87.10% | 88.14% | Baseline |

---

## 🛡️ Submitted Artifacts
1. `VaishnaviGondal_NetworkIntrusionDetection.ipynb` — Full source code notebook.
2. `requirements.txt` — Project environment dependencies.
3. `VaishnaviGondal_ProjectReport.docx` — Complete academic and technical project report.
4. `README.md` — Project summary, architecture, and run instructions.

---
**Acknowledged by BharatCares & IBM SkillsBuild Cyber Security Program 2026**
