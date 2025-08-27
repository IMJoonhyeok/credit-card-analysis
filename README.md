# 💳 신용카드 고객 데이터 분석

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"> <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white">

---

## 프로젝트 개요

### 분석 목표

신용카드 고객 데이터를 활용하여 **고객 세분화 및 인사이트 도출**을 목표로 한다.

* 주요 고객 특성을 파악하고 행동 패턴에 따라 **클러스터링 기반 세그먼트** 도출
* 고객 유지 및 마케팅 전략에 필요한 **데이터 기반 의사결정 지원**

### 활용 데이터

* **데이터 출처**: Kaggle Credit Card Dataset for Clustering
* **주요 컬럼**: 고객 ID, 신용한도, 잔액, 거래 횟수, 평균 거래 금액 등
* **데이터 크기**: 약 9,000명의 고객 데이터

---

## 분석 과정 및 주요 결과

### 데이터 전처리

* **결측치 처리** 및 이상치 제거
* 중복 데이터 확인 및 불필요한 변수 제거
* 스케일링(StandardScaler) 적용으로 변수 단위 정규화

### 탐색적 데이터 분석 (EDA)

* 변수 간 상관관계 분석 및 시각화
* 주요 변수 분포 파악 (거래 패턴, 신용한도 등)

### 차원 축소 및 군집화

* \*\*PCA(주성분 분석)\*\*를 통한 변수 차원 축소
* **K-means 클러스터링**으로 고객 세분화 (최적 군집 수 선정)
* 각 군집별 주요 특성 분석 및 인사이트 도출

### 마케팅 전략 제안

1. **고가치 고객**: 높은 한도 및 잦은 사용 → VIP 서비스 및 리워드 강화
2. **저활동 고객**: 낮은 거래 빈도 → 프로모션 제공으로 사용 유도
3. **고위험 고객**: 높은 잔액 유지 및 낮은 상환율 → 신용 리스크 관리 강화

---

## 개선 및 추가 작업

* 군집 결과를 시각화 대시보드로 확장 (Tableau, Power BI 등)
* 모델 성능 비교 (DBSCAN, Hierarchical Clustering 등) 추가 검토
* 고객 행동 로그 데이터와 통합하여 **고객 생애 가치(LTV)** 예측 가능성 검토

---

## Directory Structure

```bash
├── README.md                     <- 프로젝트 요약 설명
├── credit_card_analysis.ipynb    <- 분석 노트북 파일

```

---

## 사용 기술 스택

* **언어**: Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
* **환경**: Jupyter Notebook
* **분석 기법**: 데이터 전처리, EDA, PCA, K-means Clustering

---

## 참고 및 출처

* Kaggle Credit Card Dataset for Clustering
* Scikit-learn 공식 문서
