# [DACON] Jeju-Local-specialties-Price-Prediction-AI-Competition
🍊제주도 특산물의 가격을 예측하는 AI 모델 개발 경진대회 

팀 : 윤기웅, 조서영 

주최: 제주특별자치도

주관: 제주테크노파크, 데이콘 

결과: 193등 ( 상위 18%) 

===========================================================================

✏️
**대회 후기** 
 - ```AUTOGLUON TIME SERIES PREDICTOR의 뛰어난 성능을 경험할 수 있었다 ```
 - MLP모델을 이용한 장기적인 시계열 데이터 예측은 성능이 감소함을 깨달았다
 - Data Interpolation에 대해 더 많은 공부가 필요함을 느꼈다
 - 특산물 각각에 대한 모델을 만들고 예측을 진행하지 못 해서 아쉽다
   
   
===========================================================================

**Feature Engineering / Data Processing** 
 - 거래가 발생하지 않는 날인 일요일, 법정 공휴일 특성 추가하기
 - 날짜 정보를 이용하여 연, 월, 일 , 요일 파생변수 추가하기
 - 월, 요일에 대한 푸리에 변환을 이용하여 주기적 특성 추가하기
 - 일요일 예측값에 대해 모두 0으로 처리하여 모델 일반화 성능 향상하기   

===========================================================================

**Models**  
 - AutoML 중 뛰어난 성능을 보이는 Autogluon
 - 최근까지 SOTA 모델로 많은 관심을 받은 Nlinear, Dlinear
 - Optuna를 이용한 XGBoost, RandomForest 
