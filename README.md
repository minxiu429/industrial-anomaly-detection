# 工业设备异常检测系统 / Industrial Equipment Anomaly Detection / 산업 장비 이상 감지 시스템

## 🧠 项目简介 | Project Overview | 프로젝트 개요

本项目基于机器学习模型，使用 Pandas 和 Scikit-learn（逻辑回归与随机森林）对工业设备运行数据进行异常检测。  
This project applies machine learning (Logistic Regression & Random Forest) using Pandas and Scikit-learn to detect anomalies in industrial equipment data.  
이 프로젝트는 Pandas 및 Scikit-learn(로지스틱 회귀 및 랜덤 포레스트)을 사용하여 산업 장비 데이터의 이상을 감지하는 머신러닝 모델입니다.

---

## 📊 数据说明 | Data Description | 데이터 설명

- 数据源：仿真生成的工业设备运行数据  
- Data source: Simulated operational data of industrial equipment  
- 데이터 출처: 산업 장비의 시뮬레이션된 운영 데이터

- 字段包括 / Fields / 포함된 항목:
  - 温度（Temperature / 온도）
  - 电压（Voltage / 전압）
  - 压力（Pressure / 압력）
  - 振动值（Vibration / 진동 값）
  - 转速（RPM / 회전 속도）
  - 是否异常（Label：0=正常，1=异常）  
    (Anomaly Label: 0 = normal, 1 = anomaly / 이상 여부: 0 = 정상, 1 = 이상)

---

## 🔍 模型流程 | Modeling Pipeline | 모델링 절차

1. 数据读取与预处理（缺失值处理、特征分离）  
   Data reading and preprocessing (handling missing values, feature separation)  
   데이터 불러오기 및 전처리 (결측값 처리, 특성 분리)

2. 模型训练与测试（逻辑回归与随机森林）  
   Model training and testing (Logistic Regression & Random Forest)  
   모델 학습 및 테스트 (로지스틱 회귀, 랜덤 포레스트)

3. 性能评估（准确率、混淆矩阵、分类报告）  
   Performance evaluation (accuracy, confusion matrix, classification report)  
   성능 평가 (정확도, 혼동 행렬, 분류 리포트)

4. 可视化展示（混淆矩阵热图）  
   Visualization (Confusion Matrix Heatmap)  
   시각화 (혼동 행렬 히트맵)

---

## ✅ 项目结果 | Results | 결과 요약

- 模型对正常数据的识别准确率达到 **90%**  
- The model achieved **90%** accuracy in detecting normal data  
- 정상 데이터에 대한 분류 정확도는 **90%**에 도달하였음

- 但对异常数据的识别效果较差（准确率为 0%）  
- However, anomaly detection performance was poor (0% accuracy)  
- 하지만 이상 데이터 감지 성능은 낮았으며 정확도는 **0%**였음

- 后续需通过优化数据采集或平衡样本比例来提升检测效果  
- Further improvements can be made by optimizing data collection or balancing class distribution  
- 향후 데이터 수집 최적화 또는 데이터 균형 조정을 통해 개선 가능