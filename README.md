##  Network Intrusion Detection Using Machine Learning

###  Problem Statement

In today’s digital era, communication networks are increasingly vulnerable to sophisticated cyber-attacks like DoS, Probe, R2L, and U2R. Traditional security systems struggle to detect such attacks in real-time.
**This project** aims to develop a Machine Learning-based Network Intrusion Detection System (NIDS) that accurately classifies network traffic and detects malicious behavior.

---

###  Proposed Solution

We built a high-performance intrusion detection system using the **XGBoost** algorithm, leveraging the **Kaggle NSL-KDD dataset**. Key steps:

* **Preprocessing:** Cleaned data, encoded categorical features, and handled class imbalance using **SMOTE**.
* **Training:** Used XGBoost and Random Forest for classification.
* **Evaluation:** Assessed using Accuracy, Precision, Recall, F1-score, ROC, and PR curves.
* **Deployment:** Built a user-friendly **Streamlit app** for real-time detection via CSV upload.
* **Platform:** Entire solution is developed and deployable via **IBM Watsonx.ai Jupyter Notebook**.

---

###  Dataset

* Source: [Kaggle - NSL-KDD Network Intrusion Detection Dataset](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)
* Features: 41 network-related attributes + 1 target label
* Attack Categories: DoS, Probe, R2L, U2R, Normal

---

###  Technologies Used

* **Languages:** Python
* **Libraries:** pandas, numpy, seaborn, matplotlib, scikit-learn, xgboost, imbalanced-learn, pickle
* **Cloud Tools:** IBM Cloud Lite, Watson Studio, IBM Cloud Object Storage
* **Deployment:** Streamlit (for UI), Pickle (for model serialization)

---

###  Model Performance

| Metric             | Score   |
| ------------------ | ------- |
| Accuracy           | \~99.2% |
| Precision (Attack) | 98%     |
| Recall (Coverage)  | 99%     |
| F1-Score           | 98.5%   |
| ROC-AUC            | >0.98   |

 **Clear separation** between attack types: DoS, Probe, R2L, U2R
 **Enhanced minority class detection** via SMOTE

---

###  Visual Outputs

*  Confusion Matrix
*  ROC Curve
*  Precision-Recall Curve
*  Feature Importance Graph (Top: `service`, `src_bytes`, `flag`)

---

###  How to Run

#### 1. Clone the repo

```bash
git clone https://github.com/<your-username>/network-intrusion-detection-ML.git
cd network-intrusion-detection-ML
```

#### 2. Install dependencies

```bash
pip install -r requirements.txt
```

> Upload your `Test_data.csv` in the UI to get attack predictions.

---

###  File Structure

```
├── dataset/
│   ├── Train_data.csv
│   └── Test_data.csv
├── app.py                 
├── NIDS_Model.ipynb       
├── xgb_nids_model.pkl     
├── Darshini_ppt.pdf       
├── README.md              
```

---

###  Internship Details

**Internship Title:** IBM SKILLSBUILD 4-WEEKS INTERNSHIP ON AI & CLOUD TECHNOLOGIES  
**Platform:** [IBM SkillsBuild](https://skillsbuild.org/)  
**Organized By:** Edunet Foundation  
**Intern:** Darshini M S  
**College:** Maharaja Institute of Technology Mysore  
**Internship Duration:** 14th July 2025 – 6th August 2025  

---

###  References

* Tavallaee et al. (2009), "Analysis of KDD CUP 99 Data Set"
* IBM Developer Article – *Building a Machine Learning NIDS*
* Scikit-learn, XGBoost, imbalanced-learn official documentation
* Kaggle Dataset: [NSL-KDD](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)

---


