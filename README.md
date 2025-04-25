# Anomaly-Based-Log-Classification-for-Intrusion-Detection
The goal of this project is to improve intrusion detection systems by accurately distinguishing between genuine attacks and user errors using log data. Using BERT and RoBERTa, this project enhances detection accuracy and reduces false positives by analyzing logs both semantically and sequentially. This approach aims to improve the early identification of suspicious activities, streamline response efforts, and minimize unnecessary alerts, ultimately boosting the efficiency and reliability of security systems.

---

## 🔍 Overview

Traditional intrusion detection systems often generate excessive false positives. This project aims to intelligently analyze log files and classify them using a combination of:
- **BERT** (Masked Log Key Prediction)
- **RoBERTa** (Contextual embedding)

---

## 📁 Dataset

We used 10 real-world log datasets (~50,000 entries) with the following features:
-Timestamp – time of event
-Agent Info – source of the log (e.g., security tool)
-Geo-location – IP origin details
-Rule Classification – identifies potential attack patterns
-Source & Destination IPs/Ports – for traffic context
-Alert Category & Message – nature of detection


Each log is labeled as:
- `1` → Attack  (True Positive)
- `0` → False Positive  (human error)

---

## ⚙️ Technologies Used

- Python  
- PyTorch  
- Hugging Face Transformers  
- Scikit-learn  
- NumPy, Pandas  
- Google Colab  

---

## 🧠 Model Architecture

1. **Preprocessing**: Cleaning and tokenizing logs  
2. **BERT**: Masked log key prediction for semantic understanding  
3. **RoBERTa**: Enhanced context representation  
4. **Classification Layer**: Final binary classification (attack or not)

---

## 📊 Results

- High classification accuracy(over 85%) with significant reduction in false positives  
- Improved log understanding via contextual embeddings  
- Robust against noisy or partial logs

---

## 🚀 Future Work

- Integrate attention mechanisms for better temporal interpretation  
- Deploy as a real-time alerting service  
- Experiment with dataset balancing and adversarial examples
-Apply techniques like SMOTE or weighted loss functions to improve handling of class imbalance.

---

