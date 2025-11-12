# 🌍⚖️ AI Ethics Assignment — Designing Responsible and Fair AI Systems

This project explores **ethical AI design**, focusing on fairness, transparency, and accountability using IBM’s **AI Fairness 360** toolkit.  
The goal is to audit and mitigate bias in real-world datasets — specifically the **COMPAS Recidivism Dataset** — and demonstrate practical ethical principles for AI.

---

## 🧠 Overview

AI systems influence decisions about credit, employment, and justice.  
Without ethical safeguards, they risk reinforcing human bias.  
This assignment follows **EU AI Ethics Guidelines** emphasizing:
- **Fairness**
- **Transparency**
- **Explainability**
- **Accountability**
- **Human agency and oversight**

---

## 📊 Dataset

**Dataset Used:** COMPAS Recidivism Dataset  
**Source:** [ProPublica Analysis](https://github.com/propublica/compas-analysis)

The dataset contains demographic and criminal history information about defendants used to predict reoffending likelihood.

---

## ⚙️ Project Structure

```
ai-ethics-assignment/
│
├── data/
│   └── compas-scores-two-years.csv
│
├── notebooks/
│   ├── 01_fairness_audit.ipynb
│
├── src/
│   └── audit_fairness.py
│
├── reports/
│   └── AI_Ethics_Assignment_Report.md
│
├── requirements.txt
└── README.md
```

---

## 🧩 Installation

```bash
# Clone the repository
git clone https://github.com/<your-username>/ai-ethics-assignment.git
cd ai-ethics-assignment

# Create a virtual environment
python -m venv venv
source venv/Scripts/activate  # on Windows

# Install dependencies
pip install -r requirements.txt
```

---

## 🚀 Usage

```bash
# Run the audit script
python src/audit_fairness.py
```

or open the notebook:

```bash
jupyter notebook notebooks/01_fairness_audit.ipynb
```

---

## 📈 Example Results

**Classification Report:**
```
              precision    recall  f1-score   support
0.0             0.68      0.74      0.71      1012
1.0             0.65      0.58      0.61       839
accuracy        0.67
```

**Fairness Metrics:**
```
Before Mitigation:
 - Mean difference: -0.097
 - Disparate impact: 0.840

After Mitigation (Reweighing):
 - Mean difference: 0.000
 - Disparate impact: 1.000
```

---

## 🧮 Tools Used

- **Python 3.12**
- **AI Fairness 360**
- **Scikit-learn**
- **Pandas / Matplotlib**
- **Jupyter Notebook**

---

## ⚖️ Ethical Guidelines Applied

- **Justice:** Ensuring equal outcomes across groups.  
- **Non-maleficence:** Avoiding harm via biased predictions.  
- **Autonomy:** Respecting individuals’ data rights.  
- **Sustainability:** Responsible compute and data use.

---

## 🪄 Author
**Bikila Keneni**  
AI for Software Engineering — PLP Academy  
© 2025

---

## 📜 License
MIT License © 2025 Bikila Keneni
