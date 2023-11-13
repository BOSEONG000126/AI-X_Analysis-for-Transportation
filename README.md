# AI-X 서울시 생활 정보기반 대중교통 수요 분석
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/e304a048-ba50-4cbb-8331-8566b280546b" width="900" height="350">


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
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/869abee1-8a7a-4e50-9679-a413db19d0b8"  width="500" height="400">

  + 서울시 지도에 노선수가 많은 지역과 적은 지역을 색칠하여 인사이트를 도출합니다.
  + 서울시 중심부에 있는 구에 노선이 많고 , 외곽에 있을수록 노선이 적습니다.
  + 이와 같은 데이터 분석으로 , 65세 고령자 또한 외곽지역이 많이 거주 하는것으로 나타났습니다.
<br/>

### [2] Heat map
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/8e752f22-cb8a-41f5-8e3c-9ffcb9304770" width="500" height="400">

  + 노선수와 각 특징데이터들의 상관관계 분석 heat map 을 나타내보았습니다.
  + 노선수와 승차 총 객수 , 택시 종사자 수 , 평균 이동시간은 0.65 이상의 강한 상관계수를 보였습니다.
<br/>

### [3] Null Hypothesis(영 가설)
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/5d2aaaa3-f267-4a69-ab6e-072272b7285b" width="700" height="350">

 + 각 상관관계가 높은 feature와 노선 수를 귀무 가설로 정의합니다.
<br/>

### [4] Linear Regression(선형 회귀)
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/58973721-e660-42a3-a88f-726174c6ef22" width="700" height="350">

 + 각 feature에 대한 선형 회귀 선을 그어 회귀선과 떨어진 지역구에 점수를 부여합니다.
<br/>

## 결론

### [1] Normalization
<img src="https://github.com/BOSEONG000126/AI-X_Analysis-of-Demand-for-Public-Transportation/assets/116350240/6d7476b9-0ae7-42d3-af03-49ca87ea8eeb" width="900" height="300">

 + 각 점수의 합에 min-max 정규화를 진행하여 순위를 나열합니다.


<br/>

### [2] Conclusion
 + 결론 총 점수가 높게 나온 강서구를 가장 적합한 지역구로 선별하였습니다.
