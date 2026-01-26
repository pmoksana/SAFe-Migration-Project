# 📖 Glossary of Technical Terms

### Shopping PBI: Bridging the Gap Between AI and Business Strategy


[Executive Summary](../README.md) | [📊 Metrics](./agile-metrics.md) | [⚖️ Risk & Mitigation](./risk-mitigation-plan.md)
---

##  Purpose
This glossary serves as a reference for stakeholders to understand the Machine Learning (ML) and Data Intelligence terminology used throughout the **Shopping Predictive Brand Intelligence (PBI)** project.

---

##  Machine Learning & AI Concepts

### **Random Forest Multi-label Classifier**
The core "brain" of the Shopping PBI. It is an ensemble learning method that operates by constructing a multitude of decision trees at training time. In our context, it predicts multiple possible "future purchases" simultaneously based on a single scan.


### **Collaborative Filtering**
A method used to make automatic predictions about the interests of a user by collecting preferences from many users. 
* *Example:* "Users who scanned Brand A also frequently scanned Brand B."

### **Model Drift**
The decay of a model's predictive power due to changes in real-world environment or consumer behavior (e.g., a sudden trend in Vegan products makes old meat-purchase data less relevant).

### **CNN (Convolutional Neural Network)**
A type of Deep Learning primarily used for visual imagery. We use this to ensure that when a user scans a barcode, the system accurately "sees" and identifies the product packaging and SKU variants.

---

##  Evaluation & Statistical Metrics

### **F1-Score**
The "Golden Metric" for PBI. It is the harmonic mean of **Precision** and **Recall**. It tells us how balanced the model is—ensuring we aren't just guessing everyone will buy everything (high recall) or being too afraid to make any prediction (high precision).

### **Precision vs. Recall**
* **Precision:** Of all the purchase predictions we made, how many were actually correct?
* **Recall:** Of all the actual purchases that happened, how many did our AI successfully predict in advance?

### **Cold Start Problem**
The challenge the AI faces when a new user or a new brand joins the Shopping platform. Since there is no historical data, the AI must use "Lookalike Modeling" to make initial guesses.

---

##  Data Architecture (Databricks Style)

### **Data Lake / Delta Lake**
A centralized repository that allows us to store all Shopping scan data at any scale. We use a "Delta Lake" approach to ensure data remains clean, reliable, and ready for AI training.


### **MLOps (Machine Learning Operations)**
The set of practices that aims to deploy and maintain machine learning models in production reliably and efficiently. It is the "DevOps" for AI.

### **API Latency**
The time it takes for the Shopping app to send a scan to our AI and receive a reward prediction back. Our target is **< 200ms** to ensure a seamless user experience.

---

##  Privacy & Compliance

### **Differential Privacy**
A system for sharing information about a dataset by describing the patterns of groups within the dataset while withholding information about individuals. This ensures **GDPR compliance**.

### **K-Anonymity**
A property possessed by anonymous data. It ensures that any individual in the Shopping dataset cannot be distinguished from at least $k-1$ other individuals.

***
*Prepared by Oksana.F, Strategic Project manager. Helping stakeholders navigate the future of Predictive Retail.*