# 🎾 Tennis Match Outcome Prediction | 网球比赛结果预测

A machine learning and ensemble learning-based system for predicting professional tennis match outcomes.  
基于机器学习与集成学习的职业网球比赛胜负预测系统。

<!-- Banner -->
<div align="center">
  <img src="Result/Banner_Tennis.png" width="100%" alt="Project Banner">
</div>

<!-- Badges -->
<div align="center">
  <img src="https://img.shields.io/github/stars/Yingurt001/Tennis-Match-Prediction" alt="Stars">
  <img src="https://img.shields.io/github/license/Yingurt001/Tennis-Match-Prediction" alt="License">
  <img src="https://img.shields.io/badge/python-3.10+-blue" alt="Python Version">
</div>

---

## 🗂️ Project Overview | 项目概览

This project develops a predictive model for professional tennis match outcomes by integrating multiple ensemble learning methods. Using historical ATP and WTA match data, we engineered features such as player performance metrics, surface-adjusted statistics, and fatigue indices, then applied model ensembles for robust predictions across different tournament types and surfaces.

本项目基于 ATP 和 WTA 历史比赛数据，通过特征工程构建球员表现指标、场地调整统计量和疲劳指数，结合多种集成学习方法实现职业网球比赛结果预测，适用于不同类型和场地的赛事。

We focus on five core tasks:
- 📊 Data acquisition and preprocessing from ATP/WTA databases  
- 🏟️ Feature engineering with surface-adjusted stats and fatigue metrics  
- 🤖 Model training using Gradient Boosting, Random Forest, Logistic Regression  
- 🧠 Ensemble learning via soft voting for performance stability  
- 📈 Model evaluation and feature importance interpretation (SHAP)  

---

## 📦 Installation | 安装方式  

``` bash
git clone https://github.com/Yingurt001/Tennis-Match-Prediction.git
cd Tennis-Match-Prediction
pip install -r requirements.txt
```



## 🎯 Dataset Description | 数据集说明

### 📌 Source 数据来源
- **ATP/WTA official match records**: player names, rankings, match dates, tournament types, surfaces, in-match statistics  
- **Coverage**: Grand Slam, Masters 1000, ATP/WTA Tour events  

### 🔑 Key Features 核心特征
- 🎯 Serve performance metrics (First Serve %, Aces, Double Faults)  
- 🛡️ Return performance indicators (Break Point Conversion, Return Points Won)  
- 🏃 Fatigue index (based on consecutive matches, travel distance, tournament stage)  
- 🏟️ Surface-adjusted win rates  

---

## ⚙️ Methodology | 方法流程

### 1️⃣ Data Preprocessing | 数据预处理
- Remove incomplete records and unify categorical formats  
- Encode court surface, tournament type, and player identifiers  
- Handle missing stats via median imputation  

### 2️⃣ Feature Engineering | 特征工程
- Calculate surface-adjusted statistics to account for performance variability  
- Build fatigue index combining rest days, travel, and match load  

### 3️⃣ Modeling | 建模
- Gradient Boosting (XGBoost / LightGBM)  
- Random Forest Classifier  
- Logistic Regression  
- Ensemble via soft voting to combine model strengths  

### 4️⃣ Evaluation | 评估
- Nested cross-validation for unbiased performance estimation  
- ROC-AUC, accuracy, precision, recall metrics  
- SHAP values for interpretability  

---

## 📊 Results | 结果展示

<p align="center">
  <img src="Result/Momentum.png" width="45%">
  <img src="Result/WeChatIMG10969.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11001.png" width="45%">
  <img src="Result/WeChatIMG11005.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11007.png" width="45%">
  <img src="Result/WeChatIMG11008.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11009.png" width="45%">
  <img src="Result/WeChatIMG11032.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11034.png" width="45%">
  <img src="Result/WeChatIMG11046.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11073.png" width="45%">
  <img src="Result/WeChatIMG11105.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11114.png" width="45%">
  <img src="Result/WeChatIMG11116.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG11147.png" width="45%">
  <img src="Result/WeChatIMG11150.png" width="45%">
</p>

<p align="center">
  <img src="Result/WeChatIMG13176.png" width="45%">
  <img src="Result/WeChatIMG14652.png" width="45%">
</p>

---


### 👨‍💻 Project Maintainers
Thanks goes to these wonderful people:
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Yingurt001">
        <img src="https://avatars.githubusercontent.com/u/214812635?v=4" width="100px;" alt="Yingurt001"/>
        <br />
        <sub><b>Ying Zhang</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Alex-TtTT">
        <img src="https://avatars.githubusercontent.com/u/223631305?v=4" width="100px;" alt="Alex-TtTT"/>
        <br />
        <sub><b>Alex Hua</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Lychee-1013z">
        <img src="https://avatars.githubusercontent.com/u/221976648?v=4" width="100px;" alt="Lychee-1013z"/>
        <br />
        <sub><b>Yuzhi Zheng</b></sub>
      </a>
    </td>
  </tr>
</table>

**Authors:** Ying Zhang, [Co-Author 1], [Co-Author 2]  
**GitHub:** @Yingurt001, @[CoAuthor1], @[CoAuthor2]  
**Email:** your_email@example.com, coauthor1@example.com, coauthor2@example.com  

---

## 🎓 Citation | 引用
If you use this work, please cite:
> Zhang, Y., [CoAuthor1], [CoAuthor2]. *Tennis Match Outcome Prediction via Ensemble Learning*. 2024.

---

<div align="center">
  <b>⭐ If you find this project useful, consider giving it a star to support our work!</b>  
  <br>  
  <em>From data cleaning to match-winning predictions — tennis analytics made smarter.</em>
</div>
