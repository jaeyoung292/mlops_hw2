Happiness Score Prediction (World Happiness Report)

1) Project Overview
본 프로젝트는 World Happiness Report 데이터를 활용해 국가별 행복도를 예측하는 다중 클래스 분류 문제를 해결합니다.
AutoML 도구인 MLJAR-supervised를 사용하여 다양한 머신러닝 모델 탐색, 하이퍼파라미터 튜닝, 피처 엔지니어링을 자동화하고,
과제 1에서 구현한 Logistic Regression 모델과의 성능을 비교하였습니다.

2) Used Tools & Libraries
Python 3.11.12
pandas 2.2.2
numpy 1.23.5
scikit-learn 1.6.1
mljar-supervised 1.0.3
matplotlib 3.10.0
seaborn 0.13.2

3) Key Features
다양한 모델 자동 탐색: LightGBM, CatBoost, Neural Network
하이퍼파라미터 튜닝 및 앙상블 자동화
주요 변수 자동 생성 (Golden Features)
시각적 리포트 제공: Leaderboard, Feature Importance, Correlation Heatmap

4) Results Summary
모델	                        Accuracy	Weighted F1	Logloss
Logistic Regression (과제 1)	0.92	    0.92	      0.3006
AutoML 앙상블	                0.896	    0.8952	    0.2683
AutoML CatBoost	              0.902	    0.9012	    0.2776

5) Insights
Logistic Regression은 해석 용이성과 높은 정확도를 제공해 정책 수립에 유용
AutoML 모델은 Logloss 기준으로 더 안정적인 확률 예측을 제공하며, 복잡한 패턴 탐색에 강점을 보임
문제 상황에 따라 정확도, 해석 가능성, 예측 신뢰도를 고려한 모델 선택이 필요함
