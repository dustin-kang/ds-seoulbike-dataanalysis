# 서울시 공영자전거 따릉이의 대여정보를 이용해 중요도 예측하기

## 1. 데이터 셋
- 기상자료개방포털 : https://data.kma.go.kr/data/grnd/selectAwsRltmList.do?pgmNo=56 (금천구의 날씨 데이터)
- 서울열린데이터 광장 : http://data.seoul.go.kr/dataList/datasetList.do
 (서울특별시 공공자전거 대여 이력 정보 2020년 1월 ~ 2020년 12월 시간별 정보)

	서울특별시 공공자전거 대여소 정보 - http://data.seoul.go.kr/dataList/OA-13252/F/1/datasetView.do

	서울특별시 공공자전거 이용정보(시간대별) - http://data.seoul.go.kr/dataList/OA-15245/F/1/datasetView.do

## 2. 과정
- 데이터 전처리
- XGBoost를 이용한 이용건수에 관해 중요한 Feature 예측

## 3. 결론
- 다른 예측모델과 0.5 정도 밖에 차이가 나지 않음
- 평균 MAE가 전체 MAE와 비슷할정도로 무난한 분포임.
- 대여 시간 피처가 가장 중요도가 높으며 대부분 오후 12시 이후부터 사용수가 증가함.
- 피쳐 중요도로는 대여시간, 주말, 강수량이 가장 높음.