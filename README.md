# 📊 Feature Engineering with Weight of Evidence (WOE) & Information Value (IV)

A hands-on tutorial and code guide for performing **Weight of Evidence (WOE)** and **Information Value (IV)**—two powerful techniques used in **credit risk modeling**, **binary classification**, and **scorecard development**.  
This repository provides a complete walkthrough of the concepts, implementation, and practical applications of WOE/IV for feature engineering.

---

## 🚀 Overview

This tutorial covers:
- ✔️ What is feature enginering
- ✔️ What WOE and IV are  
- ✔️ Why they are used in predictive modeling  
- ✔️ How to calculate WOE/IV from scratch  
- ✔️ How to apply binning (manual & automatic)  
- ✔️ How to transform your dataset using WOE  
- ✔️ How to assess feature predictiveness using IV  
- ✔️ Pitfalls and best practices  

---

## 📁 Repository Structure
```
feature_engineering_woe_iv/
│
├── data/
│   └── sample_data.csv
│
├── notebooks/
│   └── feature_engineering_woe_iv.ipynb
│
├── scripts/
│   ├── __init__.py
│   └── data_loader.py
│
├── README.md
└── requirements.txt
```





---

## 📘 What Are WOE and IV?

### **Weight of Evidence (WOE)**  
A numeric transformation that expresses how well a feature separates two classes (good vs. bad outcomes).

Formula:

 WOE = ln( distribution_good / distribution_bad )

### interpreting WOE Values

- Positive WOE: Indicates that a segment has a higher proportion of non-events compared 
to events, suggesting it's a "good" predictor.

- Negative WOE: Suggests a higher proportion of events than non-events, making it a "bad" predictor.

- WOE near Zero: The segment behaves similarly to the overall population.








### **Information Value (IV)**  
A metric that quantifies a feature’s predictive power for a binary target.

| IV Value | Predictive Power        |
|----------|--------------------------|
| < 0.02   | Useless                 |
| 0.02–0.1 | Weak                    |
| 0.1–0.3  | Medium                  |
| 0.3–0.5  | Strong                  |
| > 0.5    | Suspiciously Powerful   |

---

## 📦 Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/feature_engineering_woe_iv.git
cd feature_engineering_woe_iv

## Install the dependencies:

pip install -r requirements.txt

## 📝 Usage
Run the tutorial notebook

```bash
jupyter notebook notebooks/feature_engineering_woe_iv.ipynb
