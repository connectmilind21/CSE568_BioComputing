# CSE568_BioComputing
Final Project Report

# 🧬 MCS Project Portfolio – Biocomputing (CSE 568)

**Author:** Milind Parab  
**Institution:** Arizona State University, Tempe, USA  
**Email:** mgparab@asu.edu

---

## 📄 Overview

This repository presents a portfolio of **three bio-inspired computing projects** focused on:

- **Negative Selection Algorithms (NSA)** for anomaly detection
- **Ant Colony Optimization (ACO)** and **Agent-Based Modeling (ABM)** for simulating collective behavior

These projects demonstrate how principles from immunology and natural swarm intelligence can be adapted for solving real-world problems such as:
- Text-based anomaly detection
- Fetal health monitoring using CTG signals
- Modeling of ant foraging behavior and decision-making

---

## 🧪 Projects

### 🔍 Project 1: Anomaly Detection in Text using Negative Selection

Inspired by the human immune system’s ability to distinguish self from non-self, this project uses the **Textor algorithm** to classify English (self) vs. non-English (non-self) strings.

- **Training Data:** 124 English text lines (from *Moby Dick*)
- **Testing Data:** 500 lines each from Hiligaynon, Middle English, Plautdietsch, Xhosa
- **Approach:** 
  - Anomaly score based on log-sum similarity to English
  - Evaluated using **ROC curves** and **AUC**
- **Key Insight:** Middle English showed lower AUC due to its similarity to modern English

📈 **Outcome:**  
The model successfully detected non-English texts as anomalies. AUC values showed high effectiveness, particularly for dissimilar languages like Xhosa and Plautdietsch.

---

### 🩺 Project 2: Fetal Health Monitoring using NSA

This project applies **Negative Selection** to detect anomalies in **Cardiotocography (CTG)** data, consisting of fetal heart rate (FHR) and uterine contraction patterns.

- **Dataset:** UC Irvine’s CTG dataset
- **Preprocessing:** Continuous features were discretized using binning
- **Model:** Textor algorithm with **r-contiguous detectors**
- **Evaluation:** ROC analysis with **AUC = 0.75** at optimal R=2

🧠 **Learning Outcome:**  
Demonstrated how NSA can adapt to medical time-series data through categorical transformation, highlighting its potential in **medical diagnostics and anomaly detection**.

---

### 🐜 Project 3: Agent-Based Modeling of Ant Foraging Behavior

This project models **collective decision-making in ant colonies** using **Agent-Based Modeling (ABM)** in Python via the **Mesa framework**.

- **Goal:** Simulate tandem running, food discovery, and recruitment
- **Comparison:** Translates an ODE-based model into an agent-based simulation
- **States:** Uncommitted, committed to Feeder A (strong), or Feeder B (weak)
- **Key Mechanics:**
  - Pheromone trail reinforcement
  - State transitions based on discovery, recruitment, and attrition rates

📊 **Conclusion:**  
The simulation showed **emergent behavior** consistent with natural systems: ants collectively favored the stronger food source (Feeder A), which was depleted faster—demonstrating self-organization through local rules.

---

## 🔧 Technologies & Tools Used

- **Python**: Data analysis, modeling
- **Mesa**: Agent-Based Modeling framework
- **Pandas, NumPy**: Data preprocessing and manipulation
- **Matplotlib, Seaborn**: Visualization
- **ROC, AUC**: Performance metrics
- **Subprocess**: Integration with external NSA (Textor) tools

---

## 🧠 Key Takeaways

- Adaptability of **bio-inspired algorithms** across domains
- Importance of **data representation** in model performance
- Real-world relevance in **cybersecurity**, **medical diagnostics**, **fraud detection**, and **optimization**

---

## 🌐 Links

- 📁 **Project Portfolio**: [Milind's Portfolio](https://olympus.mygreatlearning.com/eportfolio)  
- 💻 **GitHub Profile**: [connectmilind](https://github.com/connectmilind21/Profile)

---

## 📚 References

1. Elberfeld & Textor: Negative selection algorithms on
