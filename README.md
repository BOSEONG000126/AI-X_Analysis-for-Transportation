# AI-X 서울시 생활 정보기반 대중교통 수요 분석
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/1f5bc6f3-d78d-4d9b-b840-c1d49c81aadf" width="900" height="350">



## Members
  * 김보성 (Team Leader)
  * 고도연 
  * 변성호
  * 박민희
  * 진석호
<br/>

## Introduction
### Background
  + 서울시의 실제 유동인구 데이터를 활용하여 적합한 노선수 증설 구 선정을 위합니다.

<br/>

## Data Analysis
### [1] Derive insights
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/4cd755cd-7fab-4200-a6f2-5a2b90b98c36"  width="500" height="400">


  + 서울시 지도에 노선수가 많은 지역과 적은 지역을 색칠하여 인사이트를 도출합니다.
  + 서울시 중심부에 있는 구에 노선이 많고 , 외곽에 있을수록 노선이 적습니다.
  + 이와 같은 데이터 분석으로 , 65세 고령자 또한 외곽지역이 많이 거주 하는것으로 나타났습니다.
<br/>

### [2] Heat map
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/b5923897-7d0a-4fad-b40b-f9245ab0ee22" width="500" height="400">


  + 노선수와 각 특징데이터들의 상관관계 분석 heat map 을 나타내보았습니다.
  + 노선수와 승차 총 객수 , 택시 종사자 수 , 평균 이동시간은 0.65 이상의 강한 상관계수를 보였습니다.
<br/>

### [3] Null Hypothesis(영 가설)
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/bc457029-ec99-418f-983b-c7a23a218d47" width="700" height="350">

 + 각 상관관계가 높은 feature와 노선 수를 귀무 가설로 정의합니다.
<br/>

### [4] Linear Regression(선형 회귀)
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/fbf64714-0555-44b9-9237-bdd4f94bd781" width="700" height="350">

 + 각 feature에 대한 선형 회귀 선을 그어 회귀선과 떨어진 지역구에 점수를 부여합니다.
<br/>

## 결론

### [1] Normalization
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/bc5ddd72-d528-4df8-9f63-c6bfa5a82a8b" width="900" height="300">

 + 각 점수의 합에 min-max 정규화를 진행하여 순위를 나열합니다.


<br/>

### [2] Conclusion
 + 결론 총 점수가 높게 나온 강서구를 가장 적합한 지역구로 선별하였습니다.
